# States

By "States", PrestaShop calls first-level administrative divisions of a country. In the United-States, they are called _states_; in Italy, it is _regioni_ (singular: _regione_); in France, it is _régions_; in the United-Kingdom, it is _regions_. \
By default, PrestaShop provides you with a set of states: 54 US states and territories, 31 Mexican _estados_, 13 Canadian provinces and territories, 34 Indonesian _provinsi_, 24 Argentinian _provincias_, 47 Japanese _todōfuken_, and 110 Italian _province_ (singular: _provincia_).

![](<../../../../.gitbook/assets/23789709 (4) (4) (3).png>)

Having states properly defined in your database helps better represent the delivery possibilities of your carriers. These states can also be essential for tax rates calculation, depending on the country. It is therefore important to enter all of a given country's administrative divisions if they are important to your carriers. You can find a list of such divisions on this Wikipedia page: [http://en.wikipedia.org/wiki/Table\_of\_administrative\_divisions\_by\_country](http://en.wikipedia.org/wiki/Table\_of\_administrative\_divisions\_by\_country).

The PrestaShop address form currently only lists states which are available for the customer to choose. Therefore, make sure to use a sensible list when adding content to your states list. That is the reason why, for instance, the list contains Italian _province_ (second-level administrative divisions) rather than _regioni_ (first-level administrative divisions).

## Adding a New State <a href="#states-addinganewstate" id="states-addinganewstate"></a>

Let's create a new state. Click the "Add new state" button to get to the creation form.

![](<../../../../.gitbook/assets/23789711 (4) (3) (3).png>)

* **Name**. The name of the state, as it should be displayed on invoices and the package. It should therefore be in the language of the state's country.
* **ISO code**. The state's ISO-3166-2 code:
  1. Go to this Wikipedia page: [http://en.wikipedia.org/wiki/ISO\_3166-2](http://en.wikipedia.org/wiki/ISO\_3166-2),
  2. Click the state's country two-letter code (in the "Entry" column of the main table of the above mentioned Wikipedia page),
  3. On that same page, find the state's code (it should be in a list on the page, or in the text for the smallest countries),
  4. If there is one, remove the country's prefix in order to keep the code under 4 characters. For instance, the full ISO 3166-2 for Devon, in the United Kingdom, is "GB-DEV". Simply use "DEV" as the state's ISO code – it already is attached to the country using PrestaShop's "Country" drop-down list (see next step).
* **Country**. Indicate its country using the drop-down list.
* **Zone**. Indicate its geographical zone using the drop down list. Pay attention not to use the wrong zone, as this can mix up PrestaShop's country and zone settings.
* **Status**. A disabled state will not be suggested as an option when a visitor wants to register and create a new account.
