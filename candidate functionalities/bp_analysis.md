6 business processes:

1. Producer Product Submission

- Trigger: A registered producer starts a new listing.
- Inputs: Name, description, category, price, quantity, availability period, farm origin. Optional: harvest date, allergens, organic certification, best-before date.
- Outcome: A product record is created and sent for validation.
- Implied rule: Only registered producers can submit.

2. Product Data Validation

- Trigger: Product submission.
- Steps: Check mandatory fields and value validity (e.g., price and quantity are valid, the availability period is coherent).
- Decision: Valid → continue. Invalid or missing → return to the producer for correction, then re-validate.
- Gap: Full validation rule set not defined (for example, is a best-before date required for perishables, and can harvest date be after best-before?).

3. Organic Certification Verification

- Trigger: Producer claims organic certification.
- Steps: Call an external or simulated certification service to verify the claim.
- Decision: Verified → continue to publication. Rejected → the producer corrects or removes the claim.
- Exception: If the service is unavailable, what happens?

4. Product Publication

- Trigger: All required information has passed validation (and certification, if claimed).
- Outcome: The product is published and visible to customers, with its stock and season status applied.

5. Producer Inventory and Seasonal Maintenance

- Trigger: The producer updates quantity or seasonal availability.
- Outcome: Stock levels and availability windows change, which feeds into process 6.

6. Automatic Availability Control

- Stock depleted: When stock reaches zero, the product becomes unavailable for new orders automatically.
- Replenishment: When stock is restocked, the product becomes available again only if the current date is within the seasonal availability period.

Availability is the combination of two independent conditions:

▎ Orderable = (stock > 0) AND (current date is within the seasonal window) AND (product is published)

A product can be in season but out of stock, or in stock but out of season. Restocking alone does not reactivate an out-of-season product. The system should evaluate both conditions on every stock or date change, not only on restock.

7. Exception Handling (cross-cutting)

This covers the verification service being unavailable or the validation failing.

Product Lifecycle (derived)

Draft → Submitted → Validating
            ├─ invalid → Needs Correction → (resubmit) → Validating
            ├─ certification pending/unavailable → (assume unorderable)
            └─ valid → Published
                         ├─ in season AND stock > 0 → Orderable
                         ├─ stock = 0 → Unavailable (auto)
                         └─ out of season → Unavailable (auto)

Resolve questions:

1. Certification service outage: Does the product publish without certification (flagged as "pending"), stay in draft, or get queued for retry?

- The product is saved in a non-public state (not orderable) while certification is pending.
- The system retries automatically with exponential backoff, for example at 1, 5, 15, and 60 minutes, then escalates to a manual review queue after a set window (say 24 hours).
- The producer is notified of the status and can optionally publish the product without the organic badge, since the rest of the listing is valid.
- The "organic" label is never displayed until the claim is verified.


2. Validation rules: What is the complete list of mandatory fields by category? Are perishable products required to have harvest and best-before dates?

Rule set per category
- Always mandatory: name, description, category, price (> 0), quantity (≥ 0, integer or defined unit), availability period (start ≤ end), farm origin.
- Conditionally mandatory: harvest date and best-before date for perishable categories; allergen declaration for categories with known allergens or when the producer flags one.
- Cross-field rules: harvest date ≤ best-before date; best-before date must be in the future at submission

  
3. Expired products: What happens when the best-before date passes or the seasonal window closes while stock remains?

- Season closes: the product automatically becomes unavailable for new orders. Stock is retained, and the product returns to availability when the next window opens. Existing orders are unaffected.
- Best-before date passes: the product is withdrawn from sale and stock is locked, not deleted. The producer is notified and may either correct the date (only if the true date is later, with a new validation) or write off the stock. Expired stock should never be reactivated.
