# Payment Preferences

The payment preferences are meant to help you decide which payment method should be available to your customers depending on the currency, the country, the group or the carrier. Do pay attention to this page if you want no suprises!

## Payment module restrictions on currencies <a href="#paymentpreferences-paymentmodulerestrictionsoncurrencies" id="paymentpreferences-paymentmodulerestrictionsoncurrencies"></a>

Depending upon the payment, the customer's choice of currency can differ. You can limit the choice of available payment methods depending on the available currencies: you may want customers to be able to pay with any currency when using PayPal, but those paying through Moneybookers should only pay using dollars, for instance.

![](<../../../.gitbook/assets/64225552 (4).png>)

By default, only your shop's default currency is available. If you need more, follow this process:

1. In the "Localization" page under the "International" menu, import the localization pack for the country which has the currency in which you are interested. For instance, USA for US Dollars, United Kingdom for UK Pound, etc.
2. In the "Currencies" page under the "Localization" menu, enabled the currencies you just imported.

If you need to restrict payment module usage according to the user's currency, simply check the boxes that apply and click on the "Save restrictions". Note that currency restrictions work in different ways depending on the payment module:

* For some, such as Cash on delivery, you cannot change their default setting.
* For others, such as Wire payment, Check Payment, Skrill, Ogone, etc., you can change any of their currency settings, except for the "Customer currency" and "Shop default currency", which stay at their default state.
* Then, for other modules such as Hipay or PayPal, you can change any of their currency settings, but you can choose only one option between "Customer currency" and "Shop default currency", not both.

The customer can set his or her currency using the drop-down menu at the top of each front office page. You can set the shop's default currency in the "Localization" page, under the "International" menu.

If you change the default currency after having configured some first products, you will have to reset the price of all these products. You should set the default currency once and for all before adding any product.

## Payment module restrictions on groups <a href="#paymentpreferences-paymentmodulerestrictionsongroups" id="paymentpreferences-paymentmodulerestrictionsongroups"></a>

You can limit the choice of available payment methods depending on the group of customers: you can have a set number of customer groups where people can have access to more payment methods than regular customers.

![](<../../../.gitbook/assets/64225553 (2) (1) (1).png>)

For instance, you could choose to have regular customers pay with PayPal, Skrill, and Hipay, while professionals would only be able to pay by bank wire. Depending on the type of customers and on your choices, customers will only pay using the methods that match with your decisions.

## Payment module restrictions on countries <a href="#paymentpreferences-paymentmodulerestrictionsoncountries" id="paymentpreferences-paymentmodulerestrictionsoncountries"></a>

You can limit the choice of payment methods according to your customer's country of origin. For instance, you could choose to accept all payment methods for customers from France, Spain and Germany, while customers from Italy, the United Kingdom and Switzerland would only be able to pay by bank wire.

![](<../../../.gitbook/assets/64225554 (3) (5).png>)

The table lists all the known countries. If one is missing, you can add it using the "Countries" page, under the "Zones" menu.

Here again, just as with currency limitations, the available options vary depending on the payment module:

* For some, the only option is your own country.
* For others, the only options are the set of countries supported by the service: Austria, Belgium, France, etc.
* All the others native payment modules should work with all countries.

Find the country you are looking for in the alphabetical list, and check the boxes to select or unselect the payment methods you want to make available to customers from that country. Once all of your settings have been configured, click on the "Save restrictions" button, found at the bottom of the table. By default, all installed payment methods are enabled for the shop's country.

## Payment module restrictions on carriers <a href="#paymentpreferences-paymentmodulerestrictionsoncarriers" id="paymentpreferences-paymentmodulerestrictionsoncarriers"></a>

You can limit the choice of available payment methods depending on your carriers.

![](<../../../.gitbook/assets/64225554 (3) (5).png>)
