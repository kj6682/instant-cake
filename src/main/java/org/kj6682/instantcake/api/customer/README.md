**Customer API**
 
The customer api exposes the services to the customer application.
It is organised as a proxy and some common classes should be added to its definition.

This api serves the needs of
* the Customer

This api interacts with the lower level services to deal with:

* **the customer orders** - customers can use the online application to pass their orders. These orders are special orders and differ from the daily shop orders.

* **the product catalog** - the shops get information from the main product catalog

* **the laboratory stock** - it might be possible for the shop application to query the state of the stock to check if an order is feasible or not.
