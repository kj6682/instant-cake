**Laboratory API**
 
The laboratory api exposes the services to the laboratory application.
It is organised as a proxy and some common classes should be added to its definition.

This api serves the needs of
* the Chef (Chef exécutif)
* the Vice (Sous-chef (adjoint))
* the Branch Chef (Chef de Partie)
* the Clerk (Commis)
* the Carrier (Livreur)

This api interacts with the lower level services to deal with:
* **the product catalog** - the laboratory is responsible for managing the product catalog, recipies and raw materials
 
* **the shop orders** -  the laboratory fires events that make evolve the routinary orders from shops (cancel, execute, deliver) 

* **the customer orders** - the laboratory fires events that make the special orders from customers evolve (cancel, execute, deliver)

* **the laboratory stock** - each order modify the state of the stock of products and raw materials of the laboratory. An order can be refused if the stock is not enough to guarantee the deliver.
 
* **the laboratory todo** - each order modify the daily productions actions of a laboratory operator.
