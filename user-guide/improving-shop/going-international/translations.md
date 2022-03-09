# Translations

The official PrestaShop translations are retrieved from [Crowdin](https://crowdin.com/project/prestashop-official), a localization management platform on which a community of volunteer translators works on no less than 80 translation projects.

{% hint style="success" %}
If you would like to contribute to the translation of PrestaShop in your language, feel free to [join the project](https://crowdin.com/project/prestashop-official).
{% endhint %}

On the **International > Translations** page, you can adapt these official translations to your needs. For example, you can change the wording chosen by the translators to something less formal and customize the text to better suit your audience and make your store even more unique.

## Selecting the type of translations to modify

Translations have been organized into 5 sections, depending on where strings appear on PrestaShop software.

![](<../../../.gitbook/assets/Untitled (3).png>)

{% hint style="info" %}
_A string is a series of characters. It can be one character long or contain several words. When a new minor or major version of PrestaShop is released, all the new strings associated with this version are added to_ [_Crowdin_](https://crowdin.com/project/prestashop-official) _to be translated by the community._
{% endhint %}

* **Back office translations:** the strings that are visible to you and your team from your store's administration panel.
* **Theme translations:** the strings visible to your customers when browsing your store.
* **Installed module translations:** the strings present in a module. Only installed modules will be listed.
* **Email translations:** the strings used in the default email templates.
* **Other translations:** the strings that haven't been identified as being from the theme or the back office yet.

Some categories have a second drop-down list to narrow your search.

Once your selection is done, select the language in which you want to modify translations and click on "Modify". A new page opens, where you can search for translations to modify.

## Searching for a specific string

![](<../../../.gitbook/assets/Untitled (4).png>)

At the top left of the page, there is a search bar that allows you to search for a specific word or string.

You can also quickly find the untranslated strings. At the top right is displayed the total number of strings in the section and the number of missing translations. The categories that contain missing translations are displayed in red in the menu on the left of the page.

## Browsing translations

![](<../../../.gitbook/assets/Untitled (5).png>)

The menu on the left of the page allows you to browse all the strings of the category. All the strings are organized into what are called "translation domains". Translation domains aim to give more context to translators, by indicating where the string appears on PrestaShop software.

To know more about translations domains, check the dedicated page on the PrestaShop project's [Content style guide](https://zeroheight.com/80a6c5a61/v/latest/p/738e72-manage-translation-domains).

## Modifying translations

To modify an existing translation or fill out a missing one, edit or add text in the field just below the string and click on one of the "Save" buttons at the top or at the bottom of the page.

Some strings use a special syntax, with variables such as `%s`, `%d`, `%product%`, etc.

If a string contains a variable, it will be replaced with a dynamic value. For example, in the string "The product (`%product%`) is no longer available.", `%product%`will be replaced with the product's name. For example, "The product (Hummingbird printed t-shirt) is no longer available." So, you should always keep the variables in your final translation.

If a string contains a variable, you should make sure that the content of that variable will be placed in the correct flow of the sentence, and avoid literal translation.

Numbered placeholders (`%1$s`, `%2$d`, etc.) enable translators to rearrange the order of the variables in the string. For example, "This is a `%1$s` `%2$d`", with `%1$s` standing for "red" and `%2$d` standing for "pen", could be translated by "C'est un `%2$s` `%1$s`" = "C'est un stylo rouge" in French.

### Translating modules&#x20;

To translate a specific module, select the "Installed module translations" option and the desired module. A new page opens, with all the module's strings.

Depending on the module that is selected, the interface could be different. Some modules are using a translation system specific to the 1.7 version, while others are still using the former system from the 1.6 version. In the end, it doesn't change anything for you, as you will be able to translate your modules in the same way.

### Translating email templates

There are two ways of modifying the translation of an email:

* **Edit the HTML version**

With this editable preview, what you see is what you get. Click on the "Edit HTML version" button. You'll be able to edit the text and the design of your email. When you're done, save.&#x20;

* **Edit the text version**

You can edit the text version of your email directly in the text field.

{% hint style="info" %}
Make sure to keep the variables (for example `{lastname}` or `{shop_name}`) in your translations. They will be replaced with the right value when the email is sent.
{% endhint %}

![](<../../../.gitbook/assets/image (51).png>)

## Resetting translations

![](<../../../.gitbook/assets/Untitled (6).png>)

To replace a custom translation with the official PrestaShop translation, click on the "Reset" button next to the string. If the field is empty, it means that no official translation is available at the moment. Don't hesitate to [contribute to the translation project](https://crowdin.com/project/prestashop-official) if you want to make your translation available to other merchants.

## Adding or updating a language

![](<../../../.gitbook/assets/Untitled (7).png>)

To add or update a language, select the language you want from the list and click on the "Add or update a language" button. If you added a new language, you can then manage it in **Localization > Languages.**

## Exporting a language

![](<../../../.gitbook/assets/image (48).png>)

You can create your own language pack using this tool, either as a way of making a backup of your translations or sharing them.

First, select the language in which you want to export translations.

Then, select the type of translations you want:

* PrestaShop translations
* Theme translations
* Installed module translations

Each category has a second drop-down list or checkboxes to narrow your selection.

Once you are done, click on the "Export" button.

## Copying translations from one language to another

![](<../../../.gitbook/assets/image (59).png>)

You can copy the content of one language to another. This is especially useful when you want to replace a theme's language with the same language from another theme.

Select the source language and theme, then the destination language and theme, click on the "Copy" button. In most cases, the language should remain the same in both drop-down lists.

If there is already a language folder for that language in the destination theme, it will be overwritten with the language and theme files you are copying. You may want to create a new language for the destination theme before copying the source language to it.
