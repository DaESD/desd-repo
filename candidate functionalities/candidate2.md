Candidate Major Functionality Two: Product Stock and Seasonal Availability Management

This functionality covers the ongoing management of published products, ensuring that their availability on the marketplace reflects the producer's current stock levels and the product's seasonal availability period.
The purpose of this functionality is to maintain accurate product availability as circumstances change. 
It allows producers to update quantities and seasonal dates while ensuring that products cannot be ordered when stock is depleted or the seasonal availability period has ended.

**In scope**
- Updating the available quantity of an existing product.
- Updating the seasonal availability period of a product.
- Automatically marking products as unavailable when their stock reaches zero.
- Restoring product availability following stock replenishment when the product remains within its seasonal availability period.
- Preventing new orders for products outside their seasonal availability periods, even when stock remains.
- Reflecting availability changes in the customer-facing marketplace.
- Maintaining consistency between product stock, seasonal dates and orderability.
- Handling changes to stock or availability dates without bypassing the initial listing's validation and certification requirements.
- 
**Out of scope**
- Managing customer orders, payments, refunds and cancellations.
- Physical inventory tracking across farms, warehouses or distribution centres.
- Predicting future stock requirements or forecasting agricultural production.
- Automatically determining harvest quantities or planning crop production.
- Managing deliveries, courier services and fulfilment.
- Dynamic pricing, sales promotions and stock-based pricing strategies.
- Managing product listings belonging to producers who are not authorised to access them.
  
**Scope boundary**
This functionality begins once a product listing has been published and continues throughout its lifecycle on the marketplace. 
It covers changes to stock quantities and seasonal dates, together with the resulting availability status. 
It ends at the point where the system has determined whether the product can be ordered. 
The processing of actual customer orders and the physical fulfilment of those orders are outside its scope
