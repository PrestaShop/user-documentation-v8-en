# Localization settings

The main page under the "Localization" menu enables you to configure the units used for your products.

## Import a localization pack <a href="#localizationsettings-importalocalizationpack" id="localizationsettings-importalocalizationpack"></a>

This section provides you with an extensive list of existing localization packs which you can import. Not only does it set your PrestaShop install with your proper local units, but it also adds many other data:

* **States**. When shipping product to a country, knowing which state it is sent to can prove important, as this might have an impact on local customs and taxes. The added states can be viewed and edited in the "States" page under the "Locations" menu.
* **Taxes**. The real importance of localization is local taxes, and they can be numerous and varied depending on the country or the state. PrestaShop provides you with a basic support for the major taxes and tax rules. The added taxes and tax rules can be viewed and edited in the "Tax" and "Tax rules" pages under the "Taxes" menu.
* **Currencies**. Foreign customers will appreciate being able to convert the prices in your shop into their own currency. You should at least have US dollars and Euros available along of your country's own currency (if not one of those two). Once added, you must activate a new currency using the "Currencies" page under the "Localization" menu, and make sure the conversion rate is correct. The added currencies can be viewed and edited in that "Currencies" page. Make sure you also set your payment methods regarding these new currencies.
*   **Languages**. All the public fields on your shop can be created in multiple languages, and it is important you do so for your products name and description, at the very least. Note that importing a language also imports its date format (d/m/Y, m/d/Y, d.m.Y, etc.), among other things. The added languages can be viewed and edited in the "Languages" page under the "Localization" menu.

    You can add a single language, without the currency, taxes and other data depending on the country, thanks to the "Translations" page.
* **Units**. Weight, dimension, volume, distance: these units are essential in order to correctly describe a product to your customer, and for your own packaging information. They can be viewed and edited on this very page, in the "Local units" section.
*   **Change the behavior of the taxes displayed to the groups**. This is not data to import but a setting that you can change when doing the importation. It will replace the price display method for your customer groups (e.g. displaying price with tax included or not according to each customer group, as found in Shop Parameters > Customer Settings > Groups, when editing or creating a group) and activate instead the tax behavior generally applying in the country, for all groups and all countries. For example, if you are importing the localization pack for the United States and you select this option, the prices will be displayed tax excluded.&#x20;

    You should select this option only if you are importing a localization pack for the default country of your shop, as it could change the tax display methods for all groups and all countries.

    ![](<../../../../.gitbook/assets/64225597 (2) (1) (1).png>)

As you can see, these additional data are optional: you can choose to import the currency and language for a given country, and not its taxes, for instance. While you should not add too many local data for fear of overwhelming both yourself and your customers with it, it may be useful to import the localization pack for your most visited countries (according to your stats).

Apart from the default units, **you cannot automatically remove all the data for a given country**; if you need to remove data, you will have to do so manually, in their respective pages under the "Localization" menu.

## Configuration <a href="#localizationsettings-configuration" id="localizationsettings-configuration"></a>

This section groups four default local settings, of prime importance:

* **Default language**. This is the main language for your shop. This setting will influence your back office's language (including the main language for your products), as well as the front office. Note that the front office's language might adapt to the setting of the customer's browser.
* **Default country**. The location of your business. If you have headquarters in many countries, use your main or original country.
* **Default currency**. The currency in which your product's prices are first set. Currencies are added by importing and activating a country's currency. Note that if you change currency after having already set a few product prices, you will have to manually update all the existing prices. Make sure to set that value once and for all.
* **Time zone**. You own time zone. This is useful for daily discount for instance: you know exactly when it starts and ends.

The "Default language" and "Default country" settings each have an additional setting:

* For "_Default language_": **Set language from browser**. PrestaShop will set the store's language depending on the language of the visitor's browser's locale code (for instance: fr\_CA gives French)
* For "_Default country_": **Set default country from browser language**. PrestaShop will set the store's country depending on the territory of the visitor's browser's locale code (for instance, fr\_CA gives Canada).

![](<../../../../.gitbook/assets/64225598 (3) (1) (4).png>)

## Local units <a href="#localizationsettings-localunits" id="localizationsettings-localunits"></a>

The physical units presented in this section (weight, distance, volume, dimension) are used both in your product sheets and for your own packaging needs – and ultimately, is essential in your relationship with your carrier.

![](<../../../../.gitbook/assets/64225599 (4) (3).png>)

These values can be set when you import the localization package for a country, but you can edit manually them afterwards. For instance, if you would rather have centiliters instead of liters for the volume unit, change the default "L" to "cL". The values should be unit symbols from the International System of Units: [http://en.wikipedia.org/wiki/International\_System\_of\_Units](http://en.wikipedia.org/wiki/International\_System\_of\_Units).

## Advanced <a href="#localizationsettings-advanced" id="localizationsettings-advanced"></a>

This last section asks you to set your server's local language and country, as ISO code:

* For the language: ISO 639-1 code ([http://en.wikipedia.org/wiki/List\_of\_ISO\_639-1\_codes](http://en.wikipedia.org/wiki/List\_of\_ISO\_639-1\_codes)).
* For the country: ISO 3166-1 Alpha 2 code ([http://en.wikipedia.org/wiki/ISO\_3166-1\_alpha-2](http://en.wikipedia.org/wiki/ISO\_3166-1\_alpha-2)).\
  \


![](<../../../../.gitbook/assets/64225600 (4) (2) (1).png>)

These values can be set when you import the localization package for a country, but you can edit them manually at any time.
