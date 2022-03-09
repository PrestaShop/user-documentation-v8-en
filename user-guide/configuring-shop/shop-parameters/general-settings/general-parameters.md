# General parameters

The "General" page features a handful of specific settings that could not fit in the other menus. They are nonetheless essential:

* **Enable SSL**. SSL means "Secure Sockets Layer", and includes TSL (for "Transport Layer Security"). Both are cryptographic Internet protocols which secure Web communications. You can read more about these protocols on Wikipedia: [http://en.wikipedia.org/wiki/Secure\_Sockets\_Layer](http://en.wikipedia.org/wiki/Secure\_Sockets\_Layer).\
  Providing an SSL connection to your shop is not only excellent for any Internet exchanges, but also a great way to reassure your customers about the safety of their own data (authentication, credit card, etc.) on your shop, as modern browsers now display visual cues showing that the connection is secured. If your hosting provider does support SSL, make sure to activate PrestaShop's SSL support, by clicking on the link. This will reveal a selector, where you should choose "Yes". SSL will be enabled on all checkout and account pages.
* **Enable SSL on all pages**. This option is only available if you have enabled SSL. When active, all the pages of your shop will be SSL-secured (and not only the checkout and account pages).
* **Increase front office security**. This adds security tokens to your shop in order to improve its security. In effect, each URL is specific to a customer's session, and cannot be used as-is on another browser, thus protecting whatever information they might have stored during that session.
* **Allow iframes on HTML fields**. The option enables you to put iframes in text fields, such as product description. Iframes are HTML elements that make it possible to load an external content into the page's own content. We recommend that you leave this option disabled unless necessary.
* **Use HTMLPurifier Library**. Customers can send information to your shop using text fields (for instance, product descriptions or customer information), but hackers can also try to use these fields to send malicious code in order to try and hack your shop. This option guarantees that any data sent to your shop is safe. You should only disable it if you know very well what you are doing.
* **Round mode**. Once taxes and discount are applied, a price can feature too many decimals, such as $42.333333333. The round mode is used throughout PrestaShop, in the front office price display as well as during the price calculation process (taxes, discount, etc.). In and off themselves, they change little to the way things are calculated, but the impact is much bigger once taken into account in the invoice total, when many items are added up to taxes and discounts.\
  There are six modes:
  * **Round up away from zero, when it is half way there**. This is the recommended mode. 42.55555555 becomes 42.56.
  * **Round down towards zero, when it is half way there**. 42.55555555 becomes 42.56.
  * **Round towards the next even value**. 42.55555555 becomes 42.56.
  * **Round towards the next odd value**. 42.55555555 becomes 42.56.
  * **Round up to the nearest value**. 42.55555555 becomes 42.56.
  * **Round down to the nearest value**. 42.55555555 becomes 42.55.
* **Round type**. This option enables you to choose the type of rounding, which can greatly impact the calculation of the total. There are three available types, in progressive order:
  * **Round on each item**. Each item price will be rounded before calculation of the total. If there are more than one of the same item, each of those will be rounded separately before calculation.
  * **Round on each line**. Each line of items will be rounded before calculation of the total.  If there are more than one of the same item, the rounding will be done on their total value.
  * **Round on the total**. The rounding will only be done on the final calculation, after the values of all items have been added up.
* **Number of decimals**. You can choose the number of decimals that the value should be rounded to. For instance, if you choose "3", 42.333333333 becomes 42.334.
* **Display brands and suppliers**.  Enable the suppliers and brands pages on your front office even when their respective modules are disabled.
* **Display best sellers**. Enable the best-sellers pages on your front office even when the "Best-selling products" module is disabled.
* **Enable Multistore**. This little option has major implications: it turns your single-shop installation of PrestaShop into a multiple stores installation. This gives you access to the new "Multistore" page in the "Advanced parameters" menu, and every administration page can be contextualized to apply its settings to either all stores, a specific group of stores, or a single store.\
  You can read more about PrestaShop's multistore feature by reading the "Managing multiple shops" chapter of this guide.
* **Main Shop Activity**. You might have set the wrong shop activity when installing PrestaShop. You can choose the correct activity here.\
  \
  ![](<../../../../.gitbook/assets/51839963 (4) (4) (3).png>)
