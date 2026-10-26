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
