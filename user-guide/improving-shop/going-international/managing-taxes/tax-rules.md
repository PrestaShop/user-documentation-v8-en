# Tax Rules

Tax rules make it so that taxes are only applied to selected countries.

By default in PrestaShop, a tax applies to all countries/states/zones. In order to apply a specific tax rate for a single country or a set of countries (and not some others), you must create a tax rule. The tax rule is then applied on a per-product basis, during the creation of the product ("Pricing" tab).

You cannot directly apply a tax to a product; you can only apply tax rules. Therefore, you must first register all relevant taxes, then create a tax rule for that tax in order to specify the countries where the tax applies, and finally set the tax rule to the product.

A few sample taxes rules are already in place, which depends on the country you chose for your shop during the installation of PrestaShop. The tax rules are set for each tax: the rules actually serve as a kind of country filter, limiting the use of that tax to a specific set of countries.

![](<../../../../.gitbook/assets/51839958 (4) (4) (4).png>)

You should edit a couple of the presented rules in order to get a better grasp of how tax rules can be set.

## Adding a new tax rule <a href="#taxrules-addinganewtaxrule" id="taxrules-addinganewtaxrule"></a>

You can add as many tax rules as needed to your PrestaShop installation. Not only that, but you should make sure that all of the needed tax rules are registered in your shop.

Creating a new tax rule is done in two steps:

1. Create the tax rule:
   * Click on the "Add new tax rules group" button.
   * In the form that appears, name the rule. Use a telling name: use the tax rule's country code, its name, maybe even its rate, so as to find it again easily. If PrestaShop already has tax rules for the target country, use their name as inspiration so as to have some consistency.\
     \
     ![](<../../../../.gitbook/assets/51839959 (1) (3).png>)\
     \

   * Select whether the rule should be enabled from the get-go or not. You can enable it later if needed.
   * Click the "Save and stay" button. The page reloads, with a table header at the bottom and a new form.\
     \

2. Specify the country and behaviors:
   * Fill in the fields from the "New tax rule" section:\
     \


![](<../../../../.gitbook/assets/51839960 (4) (4) (1).png>)

*
  *
    * **Country**. The target country for the rule you are creating.
      * _State._ Some countries have federal states registered in PrestaShop (see the "States" page, under the "Localization" menu). In that case, you can make the tax even more specific, or choose to have it applied to the whole country. You can select more than one state by pressing the Ctrl key when clicking on state names.
    * **Zip/postal code range**. Whether the country has registered states or not, you can further specify the tax application using the customer's zip code. This field enables you to define zip codes in which the tax should be applied: either enter a single zip code or define a range using the dash. For instance, use "75000-75012" to create a range for all zip codes between these two.
    * **Behavior**. Some customers might have an address that matches more than one of your tax rules. In that case, you can choose how this tax rule should behave:
      * _This Tax Only_. Will apply only this tax, not any of the other matching taxes.
      * _Combine._ Combine taxes. For instance: 100€ + (10% + 5% => 15%) => 115€.
      * _One After Another._ Apply taxes one after another. For instance: 100€ + 10% => 110€ + 5% => 115.5€.
    * **Tax.** The tax to be used for this tax rule. That tax must already be registered in PrestaShop. If not: choose "No tax", disable the tax rule, save it, go create a tax on the "Taxes" page, then come back to edit the tax rule.
    * **Description**. You may add a short text as a reminder of why this tax rule exists for this country.
  * Click on "Save and stay". The country is added to the table below, and you can start adding another country to this tax rule group by clicking "Add a new tax rule".

Note that the default rate applied to your products will be based on your store's default country.
