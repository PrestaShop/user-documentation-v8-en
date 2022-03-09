# Countries

Your PrestaShop installation must know all existing countries in order for your customers to clearly indicate where in the world they live.

There are roughly 200 countries in the World, but PrestaShop has 244 registered. This is because some countries include overseas regions are part of the country proper. For instance, the French departments formerly known as DOM (Guadeloupe, Martinique, Mayotte, Reunion, and French Guiana) nowadays have equal status as the French metropolitan region. Likewise, Alaska and Hawaii are US States proper. Still, sending a package to Guadeloupe does not mean sending it to France, if only for the shipping fees. Therefore, the list of countries in PrestaShop actually separates the country from the mainland.

By default, only your own country is enabled in the country list. You should enable them one by one, as needed for your customers. If you are unsure which to enable, check your stats to see the countries with most visitors.

At the bottom of the list, the "Country options" section makes it possible to only display on your front office the countries that your carriers cover. We recommend that you enable this setting as it prevents customers from having to scroll through all the country names to find their own.

![](<../../../../.gitbook/assets/51839946 (4) (4) (1).png>)

## Adding a New Country <a href="#countries-addinganewcountry" id="countries-addinganewcountry"></a>

Normally, PrestaShop comes with all current countries in the database. But in the case new ones are created, you would need to add a new country.

![](<../../../../.gitbook/assets/51839947 (4) (4) (1).png>)

* **Country**. The official name of the country that you would like to add, in all supported languages. Check the country's Wikipedia page if unsure about the name.
* **ISO code**. The country's ISO-3166 code, which you can find on the official ISO page: [http://www.iso.org/iso/country\_codes/iso\_3166\_code\_lists/country\_names\_and\_code\_elements.htm](http://www.iso.org/iso/country\_codes/iso\_3166\_code\_lists/country\_names\_and\_code\_elements.htm).
* **Call prefix**. Its international call code, which you can find on [Wikipedia](http://en.wikipedia.org/wiki/List\_of\_country\_calling\_codes).
* **Default currency**. You can use your shop's default currency (as set in the "Localization" page, under the "Localization" menu), or one of the other installed currencies. Remember that if needed, you can add a new currency to your shop using the "Currencies" page.
* **Zone**. The world's subregion to which this country is attached. If necessary, you can add new zones using the "Zones" page, under the "Location" menu.
* **Does it need zip/postal code?**. Indicates whether a user living in this country must give a zip code or not when signing up to your shop.
* **Zip/post code format**. You may also give more detail on the format of the postal code (or zip code). If you do not put anything, PrestaShop will not verify the validity of the zip code when given a new address for this country. Use the following codes for the postal code: "L" for one letter, "N" for one number and "C" for the country's ISO code (the one which you entered in the ISO field above).\
  If you do not know the country's postal code format, you can rely on [Wikipedia](http://en.wikipedia.org/wiki/List\_of\_postal\_codes). Make sure you do NOT copy/paste the notation from Wikipedia, but to adapt it! For instance, Wikipedia indicates "AAA 9999\*" for Malta, so the notation for PrestaShop becomes "LLL NNNN" (without the final \*).
* **Address format**. Give details about the address layout, when displaying it to customers. You can click on the various helper links on the side of the text-field in order to add more fields. In live usage, they are automatically replaced by PrestaShop with the data from the customer's account. Your changes are only saved when you save the whole page. If you have made a mistake, you can make use of one of the four helper buttons at the bottom of the form, depending on your situation.
* **Active**. A disabled country will not be suggested as an option when a visitor wants to register and create a new account.
* **Contains states**. Indicates whether the country has "states" or not. This adds a new field to the PrestaShop address form. Note that "states" can be regions, provinces, departments... anything that makes sense to that country's postal service.
* **Do you need a tax identification number?**. A Tax Identification Number is an identification number used by the country's revenue service in the administration of tax laws. Not every country needs of even has such a number for business. Inquire about this with the country's revenue service.
* **Display tax label (e.g. "Tax** incl**.")**. **** Choose whether the tax status (included or excluded) should be displayed next to the prices or not.
* **Shop association**. You can make the country only available to a selection of your shops, for instance shops that target a specific locale.
