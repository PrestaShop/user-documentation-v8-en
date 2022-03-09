# Carriers

You must have carriers added to your PrestaShop installation – that is, a clear indicator of who will deliver your products. It might be just yourself or your shop (for instance if you are selling downloadable products, or only work locally), but as soon as you are actually sending packages using stamps and a 3rd-party delivery such as your local postal service, or FedEx, UPS and such, then you must have their details added to your shop's database. This will enable your customers to better choose which carrier to use, based on their delivery ranges, fees, and dates.

The "Carriers" page presents you with a list of all your current carriers. From there, you can directly change their status, indicate why of shipping is free or not, and change their position when presented to customers.

![](<../../../.gitbook/assets/51839919 (4) (2) (3).png>)

By default, you have two carriers in your database:

* Your own shop: This represents your physical store, where customers can supposedly come and pick up their products themselves. It has no price range or weight range set.
* "My carrier": This is a sample carrier and should not be used in production. It has one price range (from $0 to $10,000) and one weight range (from 0 kg to 10,000 kg).

It is up to you to remove these default carriers and add new ones for your customers. At the very least, you should edit the "My carrier" carrier and replace its data with that of a real carrier: name, details, and ranges. We do recommend that you delete the "My carrier" carrier, and that you use an existing carrier module in order to register you shipping partner in PrestaShop.

Video - 6 tips for creating a delivery policy that attracts customers and builds loyalty

[![](<../../../.gitbook/assets/51839792 (7) (7) (4).png>)](https://www.youtube.com/watch?v=QhTU\_eSrm7o\&list=PLyZYn1MMU7-xT-L\_zUyGnRBJmAuP6uc-c\&index=26)

\
Adding a Carrier using a recommended Carrier Module <a href="#carriers-addingacarrierusingarecommendedcarriermodule" id="carriers-addingacarrierusingarecommendedcarriermodule"></a>
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

PrestaShop comes with a host of free modules, amongst which you can find a handful of carrier modules which you can install right away, for the major worldwide and domestic carriers.

The available carriers depend on the initial settings of your shop: if you have set your shop as being located in France, you will not get the same modules as if you set your shop in the USA!

In the "Carriers" page, you can choose between creating a carrier using the Carrier Wizard, or using one of our recommended carrier modules. It is highly recommended to register carriers by installing a carrier module: this will make the process much faster, and the settings will be much more accurate.

Depending on the module, you can either click on the "Install" button and let PrestaShop do the work, or click on the shopping cart button. In that second case, you will be taken to the Addons marketplace, where you can buy the module. Once you have bought the module, you can install it and configure it.

## Adding a new carrier using the Carrier Wizard <a href="#carriers-addinganewcarrierusingthecarrierwizard" id="carriers-addinganewcarrierusingthecarrierwizard"></a>

If you cannot find a module for your shipping partner, either in the native modules or on the PrestaShop Addons marketplace, then you should register your carrier yourself using the Carrier Wizard: click on "Add new carrier" to open this tool.

In this section, we are going to create a complete carrier, from A to Z, using the Carrier Wizard. You can create as many carriers as you wish.\
If one carrier has different shipping services, you should create as many carriers in PrestaShop, and differentiate them with their names:

Many of the details asked by PrestaShop's forms should be provided by your carriers once you have set up an account or are under contract with them directly. Check with them in order to make sure everything is configured correctly.

To create a new carrier, click on the "Add new" button in the "Carriers" page. This will open the Carrier Wizard on the first of its four panels.

### Panel 1: General settings <a href="#carriers-panel1-generalsettings" id="carriers-panel1-generalsettings"></a>

This is where you describe the carrier, giving information that the customer will need in order to recognize and choose the carrier she/he prefers.

![](<../../../.gitbook/assets/51839920 (4) (4) (3).png>)

Let's examine all of the information you need to enter:

* **Carrier name**. The name is public, so you should use the official name. If you have created one PrestaShop carrier per shipping services from a single carrier, the name will help you differentiate them. \
  You could also add a description of the service. For instance, you could fill in "PrestaShipping – 500 lbs and over".
* **Transit time**. The estimated time it takes this carrier to deliver your products, written in plain language. This is displayed to customers during checkout. It will help them select their carrier according to the amount of time they are willing to wait to receive their shipment. Customers can often accept to pay more for a faster carrier.\
  You must fill this field in all the available languages, especially the default one.
* **Speed grade**. Since the "Transit time" field can contain any text, it cannot be used to compare the carriers' transit times. The "Speed grade" setting enables you to give the carrier a grade, from 0 (very slow) to 9 (very fast). This is then used to sort carriers by their speed grade, and help customers choose the one they prefer.
* **Logo**. Having a logo helps customers choose between different carriers more easily. PrestaShop will resize your image in order to fit in the checkout page.\
  The logo will appear in each panel of the Carrier Wizard, as a reminder of which carrier you are editing/creating.
* **Tracking URL**. This field must be filled with the tracking URL provided by your carrier (if there exists one). Indicate "@" where the tracking number will appear. For example, France's postal service (La Poste) offers this URL: [`http://www.colissimo.fr/portail_colissimo/suivreResultat.do?parcelnumber=@`](http://www.colissimo.fr/portail\_colissimo/suivreResultat.do?parcelnumber=@). When customers finish their purchase, they will receive that URL with the "@" replaced by the tracking number provided by the carrier, making it possible to click that link and see where the delivery process is at.

Click "Next" to reach the second panel.

### Panel 2: Shipping locations and costs <a href="#carriers-panel2-shippinglocationsandcosts" id="carriers-panel2-shippinglocationsandcosts"></a>

![](<../../../.gitbook/assets/51839921 (4) (4) (3).png>)

First, this panel presents a handful of settings:

* **Add handling costs**. Include or exclude shipping & handling costs in this carrier's price, as set in the "Preferences" page ("Handling charges").
* **Free shipping**. If enabled, you will not be able to indicate shipping prices.\
  If disabled, you will be able to edit the ranges and per-country costs in the form below.
* **Billing**. When billing the customer, PrestaShop can apply one of two behaviors, which you have to set depending on how your carrier handles billing (so make sure to check their documentation about this):\

  * **According to total price**. Billing depends on the total price of the order.
  * **According to total weight**. Billing depends on the total weight of the order.
* **Tax**. Indicates if this carrier requires a local tax in order to deliver, and if so, which one. The tax must already exist in PrestaShop (which can be done in the "Taxes" page of the "International" menu).
* **Out-of-range behavior**. In case the chosen carrier has not set any shipping cost for the required zone or weight, you can indicate how PrestaShop should react. You have two options:
  * **Apply the cost of the highest defined range**. PrestaShop will take the most costly range and apply its conditions.
  * **Disable carrier**. PrestaShop will not suggest this carrier, since it probably cannot deliver this order.

Then comes the important part: the creation of the carrier's range. This is a very important step, as PrestaShop needs this information to present the customer with carriers which can actually deliver the ordered package. Indeed, depending on the order's total price or total weight, some carrier options will not be available while others will only appear at a certain value. You must be very precise when filling these values, and preferably those suggested by each carrier's documentation.

This is where the whole Carrier Wizard takes its name. Here, you will build your carrier's price or weight ranges (depending on your choice for the "Billing" option above), one range after the other, applying your prices for each zone along the way.

Zones must have been defined beforehand. For this, go to the "Locations" page in the "International" menu.

For each range, you only need a couple of steps:

1.  **Fix the lower and upper limits of the range you are creating**. Depending on the "Billing" choice, it will display either "Will be applied when the price is" or "Will be applied when the weight is" for the lower limit, and either "Will be applied when the price is" or "Will be applied when the weight is" for the upper limit.

    Note that the lower limit is inclusive (>=) whereas the upper limit is exclusive (<). This means that a range's upper limit can have the same value as the next range's lower value, as the two will not overlap.
2. **Fill in the prices**. As soon as both lower and upper limits are filled, PrestaShop makes the "All" field available to edit. This is a special field: any value you enter in it will be copied into the field for all the available geographical zones, without any action on your part. To edit it, tick the checkbox then enter your value. You can then edit the values of each zone field separately.\
   Check the checkbox for each zone the carrier delivers to at this range. If this carrier does not make deliveries in a given geographical zone for this current range, make sure to uncheck its checkbox.
3. **Create the range**. To create another range, click the "Add new range" button. PrestaShop will add a new column of zone fields. Start again by fixing the lower and upper limits of this range, then filling the prices per zone.

The weight and price units are the default ones for your PrestaShop installation, and the ones your products use. You can change these units in the "Localization" page of the "International" menu.

Click "Next" to reach the third panel.

### Panel 3: Size, weight and group access <a href="#carriers-panel3-size-weightandgroupaccess" id="carriers-panel3-size-weightandgroupaccess"></a>

![](<../../../.gitbook/assets/51839922 (4) (4) (3).png>)

This panel presents two sets of options:

* **Maximum package height/width/depth/weight**. You can now indicate the minimum and maximum package height and weight, which are an essential part of choosing a package carrier. The value is to use the default weight and dimension units, as set in the "Localization" page of the "International" menu.
* **Group access**. You might want only some user groups to be able to use a carrier. This option serves this purpose.

Click "Next" to reach the fourth and final panel.

### Panel 4: Summary <a href="#carriers-panel4-summary" id="carriers-panel4-summary"></a>

![](<../../../.gitbook/assets/51839923 (4) (4) (3).png>)

This last panel gives you an overview of your settings for this carrier.

If some settings are wrong, you can go back to any previous panel by either using the "Previous" button or directly clicking on the panel's tab. \
If you want to save this carrier as a draft for now, then come back to it later, disable the carrier using the "Enabled" option at the bottom of this final panel. \
Either way, click on the "Finish" button to save your work, and create the carrier.

When using PrestaShop in multistore mode, another panel is available, and the panel order changes slightly:

1. General settings
2. **MultiStore**
3. Shipping locations and costs
4. Size, weight, and group access
5. Summary

All the panels are as described above. The new one, "MultiStore", makes it possible for you to limit this carrier to a selection of your stores.
