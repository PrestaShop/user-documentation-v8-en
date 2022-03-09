# Taxes

This page lists all the taxes already created in your shop. It allows you to also create new taxes if needed. For each tax, you will see its name, rate, and status. You can activate or deactivate it right from the tax list, or you can edit or delete a tax using the action button at the far right.

![](<../../../../.gitbook/assets/64225614 (4) (4) (3).png>)

## Tax options <a href="#taxes-en-taxoptions" id="taxes-en-taxoptions"></a>

At the bottom of the page is the "Tax options" section. These options apply to the whole shop and to all of the orders.

![](<../../../../.gitbook/assets/64225615 (4) (4) (2).png>)

* **Enable tax**. Whether or not taxes are included in each purchase.
* **Display tax in the shopping cart**. You might prefer the customer not to be aware of the taxes that are applied to the order. In that case, disable this option.
* **Based on**. The customer can choose to have the product not delivered at the same address as the one the order invoice should be sent to. This can have a great impact on taxes. By default, PrestaShop bases its tax rates on the delivery address, but you can choose to have them based on the billing address.
* **Use ecotax**. The ecotax refers to "taxes intended to promote ecologically sustainable activities via economic incentives". It is a tax that shop owners pay in order to "feel the social burden of their actions". Learn more about ecotax on [Wikipedia](http://en.wikipedia.org/wiki/Ecotax). Once you have enabled the use of ecotax, all your products' back office page will feature an "Ecotax (tax incl.)" field in their "Pricing" tab. You should fill that field with the exact value of the tax, which depends on your country's tax laws (it is probably based on the product's price).
* **Ecotax**. If you have enabled the use of the ecotax, a new field will appear with a drop-down list. Indeed, depending on your country's tax laws, the ecotax might be subject to VAT, hence this field to allow you to choose the associated VAT rate. &#x20;

If you decide to enable the ecotax after having added products, you will have to edit them all in order to set the tax properly for each product. Note that if you have set ecotaxes for your products already, and that you choose to disable ecotax, then all your products will lose their ecotax settings. Re-enabling the ecotax will mean having to set all your products' ecotaxes again. The ecotax will also appear to the customer, on the product's page.

## Adding a new tax <a href="#taxes-en-addinganewtax" id="taxes-en-addinganewtax"></a>

Adding a new tax is very easy because tax rules take out all the burden of having to specify the countries where the tax applies. The tax creation form is therefore very short:

* **Name**. Be very specific, as this will help you build tax rules faster. We recommend adding reminders within the name, such as the country/group/zone the tax applies to, and its rate. It helps you remember which tax is to be used in a tax rule.
* **Rate**. The exact rate, in the XX.XX format.
* **Enable**. You can disable and re-enable a tax at any time.
