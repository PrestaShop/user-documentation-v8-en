# Managing Product Attributes

Attributes are the basis of product variations (or "combinations" in PrestaShop's interface): you can only create variations of a product if at least one of its attributes changes. You should think of attributes as properties of a product that may change between variations while still keeping the same product name: color, capacity, size, weight, etc. You can use anything that varies between versions of the same product, except the price.

The difference between an attribute and a feature depends on the product itself. Some products might share the same property, one being an attribute built for building product variations, another one being simply an invariable feature. For instance, a customer can buy an iPad variation based on attributes (color, disk space) but not on features (weight, size).

Likewise, another shop might sell t-shirts variations based on attributes (color, size, gender) but not on features (weight). In your shop, features are displayed in a table, giving additional information about the product; while attributes make it possible to select among product combinations.

Attributes are configured on a per-product basis, from the "Products" page under the "Catalog" menu. However, they must first be registered on your shop using the tool on the "Attributes" tab of the "Attributes & Features" page, under the "Catalog" menu.

This page presents a list of all your currently registered attributes. You can edit or delete each one using the actions on the right of the table, or display their values by clicking on the "View" action, which opens a new table.

![](<../../../.gitbook/assets/51839263 (3) (3) (1).png>)

You can also set the attributes front office presentation order by clicking on the arrow icons, or by drag-and-dropping each row when the mouse hovers the "Position" column.

## Creating attributes <a href="#managingproductattributes-creatingattributes" id="managingproductattributes-creatingattributes"></a>

To add an attribute, or in other words, to add a group of variation possibilities (colors, capacity, material, etc.), click on "Add new attribute". A new page appears.

![](<../../../.gitbook/assets/64225526 (3) (3).png>)

Fill out the form:

* **Name**. The exact description of the attribute. This needs to be short but precise, so as to not confuse it with another attribute.
* **Public name**. The attribute name, as displayed to the customers on the product page. Since some attributes might have the same name for varying content, this field enables you to still present it correctly within the product's context, while being able to easily tell an attribute from another with a similar name but different meaning.
* **URL.** Define the URL of the attribute's page.
* **Meta title.** Give this page a title.
* **Indexable.** Activate to index this page in the Faceted Search module.
* **Attribute type**. Enables you to choose whether the product's page should display this attribute's values as a drop-down list, a radio button list, or a color (or texture) picker.

Save your new attribute to return to the attributes list. You must now add values to your attribute.

## Creating a new value <a href="#managingproductattributes-creatinganewvalue" id="managingproductattributes-creatinganewvalue"></a>

Click on "Add new value". A new page appears.

![](<../../../.gitbook/assets/64225527 (3) (3).png>)

Fill out the form:

* **Attribute group**. From the drop-down list, select one of the available attributes.
* **Value**. Give a value to the attribute: "Red", "16 Gb", "1.21 gigawatts", etc.
* **URL.** Define the URL of the attribute's value's page.
* **Meta title.** Give this page a title.

The next fields are only shown if the attribute is a color type.

* **Color**. If the attribute is a color, you can enter its value in HTML color code (i.e. "#79ff52" or "lightblue"), or use the color picker to precisely show the correct hue.
* **Texture**. If your product does not use a solid color but rather a textured one (i.e. tiger stripes), you can upload a small image file that will be displayed on the product's page. Note that this will replace the HTML color from the field above. Click on the "Save" button is order to start the upload.\
  You can also use this option to let the customer choose the color variety from a picture of your product rather than a color. How it is displayed on the front-end depends on the theme you are using...
* **Current texture**. Once you have uploaded a texture file, it is displayed in this section as a reminder.

You can add more values for the same attribute type by saving your changes with the "Save then add another value" button. Once your attributes are in place and their values are set, you can create product variations (or "combinations") in each product's "Combinations" tab, from the "Products" page under the "Catalog" menu.
