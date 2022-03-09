# Managing Categories

Categories are essential, they enable you to group equivalent products. This helps customers find their way through the variety of your catalog, and narrow down their search when looking for a specific type of product. You should create a new category from the moment you have at least two products with equivalent attributes. Products in a category should be comparable, if not interchangeable. Keep this idea in mind when adding new products and creating new categories.

Categories are determinant of how people will navigate on your site and search for your products. You should focus on your category tree and how categories are organized even before you start creating product sheets.

Categories are managed in the "Categories" page of the "Catalog" menu. This page displays a table with the currently existing categories, with the main information displayed. In order to display sub-categories, click on the parent category or select "View" in the action menu.

![](<../../../.gitbook/assets/64225507 (3) (3) (2).png>)

Thanks to the icon in the "Displayed" column of the table, you can indicate the ones you want to hide from the customer by clicking on the green check-mark icon, thus turning it into a red "x" mark.

All the categories are actually sub-categories of the "Home" category. And to edit the "Home" category (or any currently selected category), click on "Edit". If you want to create a new category (or a sub-category of an existing category), click on the "Add new category" button from any level of categories.

![](<../../../.gitbook/assets/64225508 (3) (3).png>)

Translate your categories!

Make sure to translate each field in every language that your shop supports. In order to do that, click on the language button next to the field, and choose the language in which you wish to edit the text.

First of all, you must enter a set of general information:

* **Name**. Give your category a name. Make it very short and descriptive, and choose your words wisely: your customers will rely on it when browsing your shop.
* **Displayed**. Indicate if it is "displayed" (i.e., whether or not it will be available to your customers). For example, you may want to postpone displaying a new category to your customers because you have not quite completed it.
* **Parent Category**. _Does not appear when creating a root category._ If you wish to create a subcategory belonging to a category other than the home page, choose the category under which it will appear. The form is the same when creating a root category or a sub-category. The only difference is that when clicking "Add new category" from a sub-level of categories, PrestaShop understands that you want to create a sub-category, and therefore sets the "Parent category" option accordingly.
* **Description**. You should fill this field, because not only will it be useful to you or your employees, but some themes might also make use of it, displaying it to your customers.
* **Category cover image**. Click on "Add file" to upload an image from your computer which will represent this category. It will appear on the category's page.
* **Category thumbnail**. Displays a small image in the parent category's page, if the theme allows it.
* **Menu thumbnails**. The category thumbnail appears in the menu as a small image representing the category, if the theme allows it.
* **SEO preview.** _New in 1.7.6!_ Display directly how your SEO configuration will look in search engine results.

![](../../../.gitbook/assets/64225645.gif)

* **Meta title.** The title that will appear on the search engines when a request is made by a customer
* **Meta description**. A presentation of your category in just a few lines, intended to capture a customer's interest. This will appear in the result pages of search engines.
* **Meta keywords**. Keywords that you must define in order to have your site referenced by search engines. You can enter several of them, separated by commas, as well as expressions, which must be indicated in quotation marks.
* **Friendly URL**. Enables you to rewrite the addresses of your categories as you wish. For example, instead of having an address such as [http://www.example.com/category.php?id\_category=3](http://www.example.com/category.php?id\_category=3), you can have [http://www.example.com/123-name-of-the-category](http://www.example.com/123-name-of-the-category). In this case, all you would need to do is indicate in the field marked "Friendly URL" the words that you wish to see appear instead of "name-of-the-category" separated by dashes.
*   **Group access**. Restricts access to the category and its products to certain shoppers. To see these categories, your shoppers must belong to a user group. For more information, check out the "Groups" tab in the "Customers settings" page, from the "Shop Parameters" menu.\
    \


    The root category is very useful in multistore mode. Imagine you have 3 stores with different or partly different products and categories: you might want to use a different root category for each store.

    The root category thus reflects the "home" category of each store so if you do not want to have the same products in the homepage category of each store, you need different root categories. This way it is easier to assign categories to each store and you can have different products in the home category.

Once you have finished configuring your category, save it, and you are ready to fill it with products.

A new category will not automatically appear in your shop's menu. To display it, you should edit the menu with the "Main menu" module (when using the default theme), or any custom module you may have to manage the menu

## Navigating and editing categories <a href="#managingcategories-navigatingandeditingcategories" id="managingcategories-navigatingandeditingcategories"></a>

The "Edit" button in the button bar enables you to edit the parent category of the currently-displayed sub-categories. This means that when you are viewing the main sub-categories, clicking the "Edit" button will enable you to edit the "Home" category.

You can click on any category in the table: this will open that category, and display all of its sub-categories. In effect, this will change the context of the interface: clicking the "Edit" button will edit the current parent category, and clicking the "Add new" button will open the category creation form with the "Parents category" option set to the current parent category.

## Importing and exporting categories <a href="#managingcategories-importingandexportingcategories" id="managingcategories-importingandexportingcategories"></a>

Besides the "Add new" and the "Edit" buttons, the list's button bar also features three buttons:

* **Export.** Enables you to download the list of all categories, in CSV format.
*   **Import.** Opens the "Advanced Parameters > Import" page, with the expect data type set to "Categories". Go to the "Understanding the Advanced Parameters" chapter to learn more about importing files. You will need your file to follow this format:

    ```
    ID;Name;Description;Position;Displayed;
    3;iPods;Now that you can buy movies from the iTunes Store and sync them to your iPod, the whole world is your theater.;1;1;
    4;Accessories;Wonderful accessories for your iPod;2;1;
    5;Laptops;The latest Intel processor, a bigger hard drive, plenty of memory, and even more new features all fit inside just one liberating inch. The new Mac laptops have the performance, power, and connectivity of a desktop computer. Without the desk part.;3;1;
    ```

    The category identifier is the ID, not the category's name. More import options are available in the "Import" page of the "Advanced parameters" menu.

## Adding products to a category <a href="#managingcategories-addingproductstoacategory" id="managingcategories-addingproductstoacategory"></a>

In order to add a product in a category, you must open the product configuration page and go to its "Categories" sections, on the "Basic Settings" tab. This is where you can set the categories to which the product belongs.

The "Home" category is a special category, where you can highlight/promote products from any other category by making them appear in the "Featured products" block. By default, you can only display 8 products on the homepage.

The "Featured products" block depends on the "Featured products" module. If you want more (or less) products on the homepage, configure this module (from the "Modules & Services" page in the "Installed Modules" menu).

Note: you do not have to remove a product from its original category in order to put it on the homepage. A product can have as many categories as needed.
