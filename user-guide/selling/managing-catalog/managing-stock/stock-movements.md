# Stock Movements

The table of stock movements provides you with a log of all the stock changes. Because it’s a history of previous stock movements, this table only has an informative role and therefore cannot be edited.

![](<../../../../.gitbook/assets/56688704 (3) (3) (2).png>)

## Movements overview <a href="#stockmovements-movementsoverview" id="stockmovements-movementsoverview"></a>

### Structure <a href="#stockmovements-structure" id="stockmovements-structure"></a>

The structure looks similar to the stock table but here each line corresponds to a change in physical quantity for a product or combination. It contains the following columns:

* Image thumbnail, to help fast visual recognition.
* Product’s name and when it’s a combination, its attributes’ values.
* Product reference. In case a combination has its own reference then it’ll be used instead of the parent’s reference.
* Movement type. It represents the reason why a product’s physical quantity has changed.
* Quantity added or removed. This delta is formatted with a + or - label to facilitate visual recognition.
* Date and time, which is the exact server timestamp when the change occurred.
* Employee, which is the name of the person responsible for the change.

\
By default, stock movements are sorted by descending date, so that the most recent stock movements are on the top.

### Stock movement types <a href="#stockmovements-stockmovementtypes" id="stockmovements-stockmovementtypes"></a>

As of version 1.7.2.0, three movement types can be created when triggered by the following events:

* Manual edition by an employee, when for instance you modify a product’s quantity inside the stock table.
* Customer order, when an order switches from a status equivalent to ‘not shipped’ to another status equivalent to ‘shipped’ (and vice-versa). For instance, when you ship an order that was under preparation, this will create a stock movement, as the physical quantity of items shipped literally leaves your warehouse.
* Returned products, when you refill a product’s stock after receiving and accepting the merchandise return.

In the last two cases, the movement type in the table becomes a hyperlink to the corresponding customer order, so you have more context about this type of movement and don’t have to cross-check timestamps between the stock movements and orders tables.

## Search and filter options <a href="#stockmovements-searchandfilteroptions" id="stockmovements-searchandfilteroptions"></a>

### Search bar <a href="#stockmovements-searchbar" id="stockmovements-searchbar"></a>

The search has exactly the same behavior as in the "[Stock](stock-overview.md)" tab.

### Advanced filters <a href="#stockmovements-advancedfilters" id="stockmovements-advancedfilters"></a>

In the ‘Movements’ tab, advanced filters contain:

* a movement type filter, which allows you, for instance, to look for stock movements related to customer orders.
* an employee filter.
* a date range filter, if you’re looking for stock movements which happened during a specific period.
* a category filter, like in the ‘Stock’ tab.
* a status filter.

![](<../../../../.gitbook/assets/56688706 (3) (3) (2).png>)
