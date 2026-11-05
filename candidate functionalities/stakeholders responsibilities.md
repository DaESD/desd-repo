1. **Registered Local Food Producer**

The registered local food producer is the primary user responsible for creating and maintaining product listings on the marketplace.

Responsibilities:
-- Create new product listings through the marketplace.
-- Submit all required product information, including: Product name and description, Product category. Price, Available quantity, Availability period, Farm origin, Harvest date, where relevant, Allergen information, where relevant, Organic certification details, if claiming organic status, Best-before date, where relevant.
-- Ensure submitted product information is accurate and complete.
-- Correct missing or invalid information when the marketplace requests changes.
-- Provide certification details when claiming that a product is organic.
-- Update product quantities when stock levels change.
-- Update seasonal availability periods when necessary.
-- Replenish stock information when additional products become available.

2.2 Customer

The customer is the end user who browses the marketplace to view products listed by producers.

Responsibilities:

Browse published product listings.

View product information, including descriptions, prices and farm origin.

Check relevant product information, such as harvest dates, allergen details, organic certification status and best-before dates.

Check whether a product is currently available.

Understand that a published listing may not necessarily be available to order.

Customers do not create or manage product listings. Their interaction with this use case is primarily through viewing published products and their current availability.

2.3 Main Marketplace System

The main marketplace system manages product listing submissions, validation and publication.

Responsibilities:

Provide an interface for producers to create and update product listings.

Receive submitted product information from producers.

Check that mandatory fields have been completed.

Validate submitted information and identify missing or invalid details.

Request corrections from the producer when validation fails.

Identify when a producer has claimed organic certification.

Send relevant certification information to the external verification service.

Process the verification response.

Handle situations where the external verification service is unavailable.

Publish a product listing once all required validation and verification checks have been successfully completed.

Make published product information visible to customers.

Display the product's current availability status.

Coordinate with the stock management functionality to maintain accurate availability information.

2.4 Stock Management System

The stock management system is responsible for maintaining product quantities and determining whether products are currently available.

Responsibilities:

Store and maintain the available quantity for each product.

Receive stock updates submitted by producers.

Monitor product quantities.

Automatically mark a product as unavailable when its stock reaches zero.

Check whether a product remains within its seasonal availability period.

Allow a product to become available again when stock is replenished, provided it is still within its seasonal availability period.

Ensure that a product outside its seasonal availability period remains unavailable, even if stock exists.

Communicate updated availability statuses to the main marketplace system.

Important distinction:

Product publication and product availability are separate statuses:

Published: The product has passed the required checks and its listing is visible on the marketplace.

Available: The product can currently be ordered because it has stock and is within its seasonal availability period.

A product can therefore remain published while being unavailable. When stock reaches zero, the listing should remain visible but its availability status should change. If stock is replenished and the seasonal period is still valid, the product can become available again.

2.5 External Organic Certification Verification Service

The external organic certification verification service is used when a producer claims that a product is organically certified.

Responsibilities:

Receive organic certification information from the main marketplace system.

Check the submitted certification details against the available certification records or verification mechanism.

Return a verification result to the marketplace system.

Indicate whether the certification information has been successfully verified.

Return an unsuccessful verification result when the submitted certification details cannot be confirmed.

Communicate when the verification service is unavailable or cannot complete a request.

The service does not create or publish product listings. It only supports the marketplace's validation process for organic certification claims.
