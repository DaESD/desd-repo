Functionality Scope:

In scope:

The system will cover the product listing lifecycle, beginning when a registered producer submits a new product which then goes through validation, publication and the subsequent availability management.

Product listing lifecycle:
The scope includes the management of product information from the first submission to the product being published on the marketplace. This contains the information needed to represent a product accurately. The system will provide a controlled process where submitted listings are assessed before becoming available to customers. The scope also covers the handling of unsuccessful submissions, making sure that incomplete or invalid listings are corrected before being published. This makes product publication a part of a managed workflow rather than an unrestricted action available immediately after data entry.

Product information and data integrity:
The scope includes maintaining the accuracy and completeness of the information associated with each product listing. This covers core product details as well as any relevant information about the product such as allergen information, organic certification and harvest dates. The system is responsible for making sure that the information is suitable for listing and remains consistent even when a producer makes changes. The scope also includes retaining product information throughout the listing lifecycle so that changes do not require the producer to recreate the entire listing.

Organic Certification verification:
The scope includes checking the organic certification status as part of the product publication process. It is performed through an external service/simulated service that represents the behaviour of a certification verification system. This includes managing the outcome of the process and accounting for situations where the details can't be confirmed. The system is responsible for handling the verification result appropriately, it isn't responsible for issuing organic certification or determine the underlying standards used by certification authorities.

Product publication and customer visibility:
The scope includes allowing eligible product listings available through the customer-facing marketplace once the required checks have been completed. This covers the link between a product's publication status and its ability to be ordered. However, published listings may be visible even when they cannot be ordered, for example, when stock has run out or the seasonal availability period ends. This falls within the scope since the system has to manage product availability without removing the listing from the marketplace.

Ongoing stock and seasonal management:
The scope includes the management of product availability after a product has been listed. Producers have to be able to maintain the information that determines whether a product can be supplied, including the current quantity and its seasonal availability period. The system manages the link between these factors so that availability reflects the product's actual supply conditions. It will also account for changes over time, including stock depletion, replenishment and the start and end of a seasonal period. This makes it so that the listing remains consistent with the producer's current ability to supply the product.

Error Handling and external dependencies:
The scope includes handling failures within the listing workflow, especially invalid submissions and any interruptions to the certification verification service. The system will need to distinguish between information which has been rejected and information that hasn't been verified. It also needs to preserve the integrity of the listing process when an external dependency fails, so that a temporary service interruption doesn't result in an incorrectly approved product.

Out of scope:
These activities are excluded from the use case chosen because they represent separate marketplace functions which are beyond the product listing lifecycle which is in use case 1.

Producer registration and account administration:
The system will not cover the creation of producer accounts, registration approval, identity verification and management of producer credentials. The use case given assumes that the producer is registered and authorised to submit their products. Even though authentication and access control is necessary for the marketplace, this particular use case begins after these prerequisites have been met.

Customer ordering and transactions:
The scope doesn't include the complete purchasing process. The workflow is responsible for providing accurate information about whether a product is available to order but doesn't implement the ordering and payment process that occurs when a customer wants to purchase an item. In a wider system, this is necessary however for this use case it is not needed.

Delivery, Distribution and fulfilment:
The system won't manage the physical movement of products. Activities such as delivery scheduling, courier allocation, shipping and dispatch confirmation are excluded. Although farm origin and seasonal availability are relevant to the listing, the use case doesn't include how products are transported, stored or delivered after an order has been placed.

Certification issuance and regulatory administration:
The system will not act as an certification authority, its responsibility is limited to checking whether the certificate is valid or not through an external service. The accuracy of the external certification service remains outside the system's control.

Advanced inventory and agricultural management:
The scope excludes wider farm management and inventory planning. The system itself will manage the available quantity associated with a marketplace listing but it won't attempt to manage the producer's entire operation or independently determine the amount of stock that needs to be produced.

Pricing strategy and financial management:
The system won't determine product prices through market analysis, competitor comparisons or dynamic pricing. Financial activities such as invoices and managing payouts are also excluded. The producer supplies the product price when listing a product. The use case doesn't define how the price is determined or how the marketplace manages the resulting transactions.

Marketing and customer engagement:
The scope excludes promotional campaigns, advertising, loyalty programmes and reviews. These features support the wider marketplace but aren't necessary to establish the product listing and availability workflow that is described in the case study.

Business intelligence and reporting:
The system won't provide advanced analytics relating to sales performance, revenue, customer behaviour, seasonal demand or producer performance. These functionalities require additional reporting requirements and data beyond what's necessary to create and maintain product listings. Basic records needed to maintain product information and verification outcomes remain within scope but the exclusion concerns the production of wider analytical reports and business insights.

Overall, the functional scope is limited to the product listing lifecycle within the marketplace, covering product information submission, data validation, organic certification verification, publication and ongoing availability management. This includes the maintenance of accurate product information and the handling of unsuccessful validation, certification verification failures and external service interruptions. The system will also manage the link between product stock, seasonal availability and eligibility for new orders, ensuring that published listings accurately reflect whether the products can be supplied or not.
The scope begins with an existing registered producer submitting a product and ends with the ongoing maintenance of the listing and its availability status. It does not include producer registration, customer transaction processing, delivery and fulfilment, certification issuance, wider farm management, automated pricing strategies, marketing or advanced business reporting. These activities are considered separate functions of the wider marketplace and are excluded from this use case unless it is introduced through additional requirements.
