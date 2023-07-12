# New product page (PrestaShop 8.1)

{% hint style="info" %}
To use the new product page, you must enable it in the [New & experimental features](../../configuring-shop/advanced-parameters/experimental-features.md) page on PrestaShop 8.1:
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (96) (1).png" alt=""><figcaption></figcaption></figure>

## Adding a new product

To add a new product to your catalog, click on **"Add new product"** from the **Catalog > Products** page.

A new window opens, displaying the **4 different types of products** you can add to your store. Selecting a specific type of product will change the different tabs displayed on the product creation page:

<figure><img src="../../../.gitbook/assets/image (43) (1).png" alt=""><figcaption></figcaption></figure>

* **Standard product:** _A physical product that needs to be shipped._ The **Stocks** tab will be shown. Note that you **cannot add combinations to a standard product**.
* **Product with combinations:** _A product with different variations (size, color, etc.) from which customers can choose._ The **Combinations** tab will be shown and the Stocks tab will disappear.&#x20;
* **Pack of products:** _A collection of products from your catalog._ The **Pack** tab will be shown and the Combinations and Stocks tabs will disappear.&#x20;
* **Virtual product:** _An intangible product that doesn't require shipping. You can also add a downloadable file._ The **Virtual product** tab will be shown and the Combinations, Stocks, and Pack tabs will disappear.

### Changing the product type

If you've selected the wrong product type, you can quickly change its type:

* Click on the **product type** (under the product name field)
* A window asking you to **select the new product type** is displayed:

<figure><img src="../../../.gitbook/assets/image (80) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Note that by changing your product type, **all combinations will be deleted** and **your stocks will be reset.**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (104).png" alt=""><figcaption></figcaption></figure>

## Creating a product with combinations

In PrestaShop 8.1, the combination page has been reworked. A combination generation modal now appears when clicking on the "**Combinations" > "Manage product combinations"** tab.

To select single values, **click on an attribute** to expand it and **select the values** you want to add to your product.

<figure><img src="../../../.gitbook/assets/image (103).png" alt=""><figcaption></figcaption></figure>

To select all combinations for each attribute, **click on the checkbox** on the left of your chosen attribute(s):

<figure><img src="../../../.gitbook/assets/image (107).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
You can also manually search for an attribute using the **"Search for attributes..."** field to find specific attributes.&#x20;

![](<../../../.gitbook/assets/image (58) (1).png>)

This feature can be useful if your catalog has a lot of different attributes.
{% endhint %}

## Generating combinations

If you select every value for the "Size" and "Color" attributes, you can generate up to 56 combinations in your catalog. Once you have selected your attributes, click on **"Generate X combinations"** to generate combinations.

When using **multistore mode**, you can generate attributes for all stores by checking the dedicated **"Generate combinations for all stores"** option, next to the "Cancel" button:

<figure><img src="../../../.gitbook/assets/image (109).png" alt=""><figcaption></figcaption></figure>

## Managing combinations

### Using combination filters

PrestaShop 8.1 introduces combinations filters on the **"Combinations" > "Manage product combinations"** page, allowing you to quickly manage combinations in your store:

<figure><img src="../../../.gitbook/assets/image (36) (1).png" alt=""><figcaption></figcaption></figure>

## Bulk actions

{% hint style="info" %}
You can use bulk actions to remove or edit quickly some or all product combinations at once.&#x20;
{% endhint %}

To select multiple elements at once, you can use filters and select the attributes you wish to edit or remove. You can also use the checkmark list on the left side of the product table to manually select your chosen items.

### Editing attributes in bulk

To edit a field in bulk, **select the combinations you wish to edit** and click on the **"Bulk actions"** button:

<figure><img src="../../../.gitbook/assets/image (102).png" alt=""><figcaption></figcaption></figure>

Then, click on the dropdown list for each category (for example, "Retail price") and select the element you wish to edit.

You can then enable the field using the slider button (enable/disable) and **type in your desired value.**

<figure><img src="../../../.gitbook/assets/image (94) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
By default, the set value for **every field is 0.**

To reset a field, you can **toggle it** and manually set its **value back to 0.**
{% endhint %}

This way, changes will only be applied to **your selected combinations.**

### Removing attributes in bulk

You can remove attributes in bulk by selecting multiple elements at once through filters or checkmarks, then click on **"Bulk actions" > "Delete X combinations"**&#x20;

![](<../../../.gitbook/assets/image (87) (1).png>)

A window is displayed asking you to **confirm your choice.**

## Pagination

{% hint style="info" %}
The new product page now includes a pagination feature. It allows you to easily browse through your store's products and display up to 100 items per page.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4) (3).png" alt=""><figcaption></figcaption></figure>

With the implementation of the pagination feature, page loading time has been greatly reduced. This means you can have as many combinations as you want and you don't have to worry about your back office's performance.

## Pricing

<figure><img src="../../../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

### Retail price

The Pricing tab now features a simple tax calculator, allowing you to quickly and clearly calculate your tax-included retail price.

To add a new tax rule to your retail price:

* Enter your **initial retail price (without tax)**,&#x20;
* Then chose the **tax rule you wish to apply** from the list.&#x20;

The product's retail price (tax included) will automatically be calculated for your product.

<figure><img src="../../../.gitbook/assets/image (65) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**I can't find a specific tax rule in the list.**

You can add tax rules for specific countries by clicking on "**Manage tax rules"** to manually add a tax rule.

You can also by [import a new localization pack](../../improving-shop/going-international/localization/localization-settings.md#localizationsettings-importalocalizationpack)'s taxes from the [Localization](../../improving-shop/going-international/localization/) page:

![](<../../../.gitbook/assets/image (51) (1).png>)
{% endhint %}

### Summary

A summary of your product's cost is now displayed so you can check your product's cost and price in detail at a glance.

<figure><img src="../../../.gitbook/assets/image (100).png" alt=""><figcaption></figcaption></figure>

As a reminder, the margin is calculated like so:

<figure><img src="https://imgr.whimsical.com/object/UQpG8dCv3DfNs8HAGxb7vz" alt=""><figcaption></figcaption></figure>

### Displaying retail price per unit

Knowing your unit retail price is useful when selling items that need to be sold per kilo or liter or any other unit.&#x20;

For example, if you sell candies per kilo in your store, you can specify the **price per kilo** and it will be displayed in your summary, under the included and excluded tax price.

Toggle the **"Display retail price per unit"** feature to display the retail price per unit on the summary.

<figure><img src="../../../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>

## Image management

### Replacing an image

You can now replace a product image. Simply select the image you wish to replace and click on the **"Replace selection"** button. Select an image on your computer and **make sure to save your changes.**

<figure><img src="../../../.gitbook/assets/image (42) (2).png" alt=""><figcaption></figcaption></figure>

### Replacing images in bulk

It is now possible to replace a product image in bulk. You don't need to worry about losing image links and data anymore.

**To replace images in bulk,**

* **Select the combinations** you wish to edit,&#x20;
* Click on the **"Bulk actions"** button and select **"Edit X combinations"**
* Go to the **"Images"** attribute and **Toggle the feature** to enable it.

You can now **select the image** you wish to associate with your combinations.

<figure><img src="../../../.gitbook/assets/image (56) (1).png" alt=""><figcaption></figcaption></figure>

### Deleting images in bulk

It's now possible to delete product images in bulk.

To do so, select the images you wish to delete and click on the **"Delete selection"** button:

<figure><img src="../../../.gitbook/assets/image (27) (2).png" alt=""><figcaption></figcaption></figure>

## Stocks

#### Edit quantity

A new stock system has been implemented. To manage your stocks, simply **add a positive number** or **subtract a negative number** in the stocks quantity field to update your stocks:

<figure><img src="https://imgr.whimsical.com/object/UH9yJk9gf9A5CWB1aJBGW1" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Clients sometimes buy products while you're updating your stocks. An incorrect stock calculation will now be avoided as you can only update your stocks by adding or subtracting products. This way, you can ensure correct and reliable stock management in your store.
{% endhint %}

#### Recent stock movements

To have a better look at your stock, a preview of the last 5 stock movements is displayed under the **"Recent stock movements"** tab.&#x20;

<figure><img src="../../../.gitbook/assets/image (24) (1).png" alt=""><figcaption></figcaption></figure>

These stock movements also include order stock movements (the sales and product returns in between 2 stock movements). &#x20;

Stock movement of customer orders is now regrouped to have a better summary of your stocks.&#x20;

<figure><img src="../../../.gitbook/assets/image (33) (1).png" alt=""><figcaption></figcaption></figure>

## Header

The header now recaps everything you need to know about your products: types, references, stock, tax, etc.) You can easily find important information about your product at a glance.

#### Color indicator

Three colors now indicate your stock status:

* **Green "in stock":** when your stock is superior to your set low stock.
* **Yellow "low stock":** when the stock is equal or inferior to set low stock&#x20;
* **Red "out of stock":** when the stock is inferior or equal to 0.

<figure><img src="https://imgr.whimsical.com/object/AfpPbkpktdee3z8Y1NSf9M" alt=""><figcaption></figcaption></figure>

## Footer

#### New wording

The footer's wording has been improved for clarity. The save button now has two states:

* **Save:** Saves your product when creating it or when the product is offline (not published) on your store.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

* **Save and publish:** Saves your product and publishes it on your store.&#x20;

<figure><img src="../../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

This helps you better understand whether your changes are live on your store or not.

### Dynamic footer

The footer is now **dynamic and reacts to your actions.**&#x20;

Modifications can be **canceled, previewed, saved, or published**:

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

For example, if you have unsaved modifications, any action that would make you leave the current page is disabled:

![](<../../../.gitbook/assets/image (72).png>)
