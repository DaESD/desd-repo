Use case 1 

User stories:
There are 4 main actors within the case study.
External Verification Service: Checks the organic certification information
System: Validates the product information submitted, verifies the certification and manages the product availability
Customer: Can view and purchase the products available to buy 
Registered Producer: Creates and manages product listings

Functional Requirements:
Product information submission
- allow registered producers to create new product listings
- allow producers to enter required product information
- allow producers to submit product information for validation

Product Validation
- system validates that product price is a positive monetary value
- if the validation fails, system prevents publication
- system retains valid information entered when producer is asked to correct an invalid field 

Product Publication
- system can only publish a product only if mandatory information has passed the verification process
- system makes product visible to customers through marketplace
- system does not display unpublished/rejected products for purchase

Stock management
- system allows producers to update available product quantity
- system marks a product as unavailable as soon as stock hits 0
- system allows product to become available once seasonal availability is over

Seasonal availability management
- allows producer to update product seasonal availability dates
- system checks if seasonal availability date is valid

Non-Functional Requirements:
- system requires producers to authenticate before creating or updating product listings
- system ensures producers can only modify products they are authorised to manage
- system preserves accurate product information, stock quantities and availability status when changes are made
- system handles verification service failures without incorrectly approving organic certification
- system provides clear verification messages which identify the problem and explain how it can be corrected
- system processes product submissions and updates within an acceptable response time under normal operating conditions
- marketplace remains operational when external certification service is temporarily unavailable
- system maintains records of product creation, updates, certification verification outcomes and changes to availability
- system ensures that customers can't place new orders for products marked as unavailable
- system should separate product validation, certification, publication and stock management so that these functions can be maintained independently

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

