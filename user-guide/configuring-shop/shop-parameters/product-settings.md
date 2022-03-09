# Product Settings

This page contains the preferences pertaining to how your products are to be handled and displayed by PrestaShop.

## General preferences <a href="#productsettings-generalpreferences" id="productsettings-generalpreferences"></a>

![](<../../../.gitbook/assets/64225486 (4).png>)

* **Catalog mode**. Enabling catalog mode turns your shop into a simple gallery of products, with no way to buy the items whatsoever.
* **Number of days for which the product is considered 'new'**. When you add a product to your shop, it is considered new and it is available on the "New products" page. The field allows you to specify how many days the product will remain visible on this page. With this feature, you choose how to display and update your shop's novelties. The "New products" page is usually most accessed by your regular customers.
* **Max size of product summary**. Your product has two descriptions: a "summary" and a regular description. The summary, which appears in search engines and in the category description for your product, is limited to 800 characters by default.
* **Quantity discount based on**. This setting indicates upon what PrestaShop should base quantity discounts: per-product, or per-combination (which can feature multiple products).
* **Force update of friendly URL**. By default, the friendly URL of a product page is generated from the product title, and it stays the same even though the product title changes – because in order to be well referenced, your URLs should be stable. By enabling this option, PrestaShop will update the friendly URL every time you change the product's name or page's title.
* **Enable by default**.  If you enable this option, new products will automatically be activated when you create them.

## Pagination preferences <a href="#productsettings-paginationpreferences" id="productsettings-paginationpreferences"></a>

![](<../../../.gitbook/assets/64225489 (4) (1) (3).png>)

* **Products per page**. Indicate how many products are displayed on the pages of your categories.
* **Default order by**. Indicate the order of products in your shop's categories. 6 choices are available:
  * _Product name._ Displays your products based on the alphabetical order.
  * _Product price._ Displays your products according to their prices.
  * _Product add date._ Displays your products according to the date it was added to your shop.
  * _Product modified date._ When you edit a product, its modification date is changed. This option makes them appear in the order of modification date.
  * _Position inside category._ Displays your products as they are positioned in the categories in your catalog. The position of the products can be modified directly in the catalog of your shop using the position arrows. This way you have your products in the most attractive fashion for your customers.
  * _Brand._ Displays your products in alphabetical order of their brands' names.
  * _Product quantity._ Displays your products based on their available quantity.
  * _Product reference._ Displays your products based on their reference number.
* **Default order method**. The above options can be sorted by ascending or descending order.

## Product page preferences <a href="#productsettings-productpagepreferences" id="productsettings-productpagepreferences"></a>

![](<../../../.gitbook/assets/64225488 (3).png>)

* **Display available quantities on the product page**. By enabling this feature, your visitors can see the quantities of each product available in stock. Displaying this information can be used to stimulate sales in the case where the quantity in stock is low. The quantities displayed are the selected attributes and combination.
* **Display remaining quantities when quantity is lower than**. You can choose to display an alert when the remaining available stock for a product gets below a certain level. This option is particularly useful for promoting purchases. The text and placement of the alert depend on the theme; in the default theme, it is "Last items in stock", and is placed next to the "Add to cart" button.
* **Display unavailable product attributes on product page**. Your products can be composed of many different combinations or attributes: color, size, capacity, etc. Attributes can be edited in the "Attributes" page of the "Catalog" menu. When one or several attributes are not available anymore, you have two possibilities:
  * _First possibility:_ Leave this preference active. Example: The "iPod Shuffle" is no longer available in "Blue" in our shop. By keeping this option enabled, the product's combination will remain visible in the shop. A message will indicate that the product is no longer available in the chosen option, and invite customers to choose another combination. If you enabled the "Allow ordering of out-of-stock products" option (see below), then they will be able to add the unavailable combination to their carts.
  * _Second possibility:_ Disable this preference. If the "Blue" combination of the "iPod Shuffle" product is no longer available, that selection is not displayed the front office and the customer cannot select it. This feature helps to clearly display the availability of your products.
* **Display the "add to cart" button when a product has attributes**. This option prevents customers from adding a product to their cart directly from the category page, if that product has combinations. This forces customers to visit the product's page and pick a combination, instead of only adding the default one to the cart. Note that products with no combination will still have an "Add to cart" button in the category page.
* **Separator of attribute anchor on the product links**. Choose the separator, between "," and "-".
* **Display discounted price**. When using the volume discount board, show the discounted price rather than the discount percentage.

## Products stock preferences <a href="#productsettings-productsstockpreferences" id="productsettings-productsstockpreferences"></a>

![](<../../../.gitbook/assets/64225490 (4) (4) (3).png>)

* **Allow ordering of out-of-stock products**. If a product does not have any available stock anymore, the customer can still order it.
* **Enable stock management**. This option gives you access to basic stock management options and features: you can set the current quantity of product, and have PrestaShop lower it for each order, and "re-stock" for each canceled or returned order. By default you should leave this feature enabled, as disabling it affects the entire inventory management of your shop. Only if you do not have any physical inventory should you disable it – for instance, if you only have virtual products.
* **Label of in-stock products.** Display a label for in-stock products.
* **Label of out-of-stock products with allowed backorders**. Display a label for out-of-stock products with allowed backorders.
* **Label of out-of-stock products with denied backorders**. Display a label for out-of-stock products with denied backorders.
* **Delivery time of in-stock products.** Recommended to Europeans merchants in order to comply with the legislation.
* **Delivery time of out-of-stock products with allowed backorders**. Recommended to Europeans merchants in order to comply with the legislation.
* **Default pack stock management**. When you sell packs of products, the way your stock is updated depends on this option. You have three possibilities:
  * _Decrement pack only._ When a pack is sold, only the stock for the pack will be impacted.
  * _Decrement products in pack only._ When a pack is sold, only the stock for each product will be impacted.
  * _Decrement both._ When a pack is sold, both the stock for the pack and the stock for each product will be impacted.

This setting can be changed for each one of your pack in their own product page, in the "Quantities" tab.
