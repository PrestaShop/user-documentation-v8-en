# Import

The import page enables you to easily fill your product catalog when you have a very large amount of products, or to import data that you exported and converted from another e-commerce tool.

Historically imports were made using .CSV files in PrestaShop. Since the version 1.7, other formats of file are supported, such as .xls, .xlsx, .xlst, .ods, and .ots.

CSV is an acronym of "Comma-separated values". It is a popular plain-text format when there is a need to import, export or simply store data in a non-proprietary format. Almost all data handling tool support CSV format, in various incarnations. You can read more about the CSV format on Wikipedia: [http://en.wikipedia.org/wiki/Comma-separated\_values](http://en.wikipedia.org/wiki/Comma-separated\_values).

![](<../../../.gitbook/assets/51840005 (3) (4).png>)

The import process requires preparation, and starts with a form made of primary settings:

* **What do you want to import?**. Choose in the drop-down list what kind of entity you would like to import to your shop. The "Available fields" on the right updates when you choose an entity, so that you know the kind of data that your import file should contain.\
  PrestaShop enables you to import the following types of data:
  * Categories,
  * Products,
  * Combinations,
  * Customers,
  * Addresses,
  * Brands,
  * Suppliers,
  * Aliases,
  * Supply orders (if Advanced Stock Management is enabled),
  * Supply order details (if Advanced Stock Management is enabled).
  * Store contacts
*   **Select a file to import**. You can import more than one file at a time, but make sure that they all contain the same type of data. You can either upload files from your computer, or choose files already available on your FTP/ in your history.

    You can download sample files for each type of data from the "Download sample CSV files" section on the right. This helps you compare these sample files with your own files, so that you can make sure that the files you are about to import are indeed ready to be imported to PrestaShop. These files are actually stored in the `/docs/csv_import` folder of your installation of PrestaShop.
* **Language of the file**. Data can only be imported for a single language at a time. If your data exists in more than one language, you should split it into as many files.
* **Field separator**. Not all CSV file use commas to separate their values: some use tabulations, others semicolons, etc. You can indicate what your files use in this field.
* **Multiple value separator**. When an attribute can support more than one value, these values need to be separated with a specific separator. After reviewing your files, indicate your separator here.
* **Delete all \_\_\_ before import**. This option will erase all previously existing entries of the type of data you are importing. Thus you will start with a clean slate.
* **Use product reference as key**. Product import only. You can choose to have the product key be determined by PrestaShop, or instead use the product's reference as the ID. In this case, make sure the file does contain references for all your imported products.
* **Skip thumbnails regeneration**. Category and product import only. You can choose to have PrestaShop regenerate the thumbnails that are linked from your CSV file (in the "Image URL" or "Image URLs" fields).
* **Force all ID numbers**. You can either keep the imported IDs, or let the importer auto-increment them.
* **Send notification email**. If you are importing large files, activate this option to receive an email when the import is complete.

When changing the entity you wish to import, the section on the right, titled "Available fields", changes to present the expected data fields. Although the importing tool helps you by taking care of matching your file's fields with PrestaShop's, you should strive to make your data more import-friendly by following the naming scheme and order of the presented fields. If not, the import will be more tedious, but not impossible.\
Some fields have a little information popup available (represented by an "i" logo), which you can display by hovering the mouse cursor over it. They mostly pertain to PrestaShop's multistore or advanced stock management features. Make sure to read them all in order to better build/edit your data files.

![](<../../../.gitbook/assets/45580389 (4) (4) (3).png>)

## Data format <a href="#import-dataformat" id="import-dataformat"></a>

Imported data file must be in text-file, using a CSV-based format and the accompanying `.csv` file extension. We recommend using a semicolon ";" as a field separator. If you textual data (product description and such) contains semicolons, you should either remove them, or choose another separator in the "Field separator" option.

You can create a CSV file using any text editor (we recommend Notepad++: [http://notepad-plus-plus.org/](http://notepad-plus-plus.org)), but we do advise you to use a spreadsheet program, then save your work in the CSV format. Using a spreadsheet program enables you to have an easier and more visual grasp of your data, in comparison to the plain text file. You can use the commercial Microsoft Excel ([http://office.microsoft.com/en-us/excel/](http://office.microsoft.com/en-us/excel/) or the free [OpenOffice.org](http://openoffice.org) [http://www.openoffice.org/](http://www.openoffice.org) Calc.

Here is a sample import file, with a list of products:

```
"Enabled";"Name";"Categories";"Price";"Tax rule ID";"Buying price";"On sale";"Reference";"Weight";"Quantity";"Short desc.";"Long desc";"Images URL"
1;"Test";"1,2,3";130;1;75;0;"PROD-TEST";"0.500";10;"'Tis a short desc.";"This is a long description.";"http://www.myprestashop/images/product1.gif"
0;"Test 02";"1,5";110;1;65;0;"PROD-TEST2";"0.500";10;"'Tis also a short desc.";"This is a long description too.";"http://www.myprestashop/images/product2.gif"
1;"Test 03";"4,5";150;1;85;0;"PROD-TEST3";"0.500";10;"'Tis a short desc. again";"This is also a long description.";"http://www.myprestashop/images/product3.gif"
```

Note that this is only a regular sample files built for this demonstration; it is purposefully not optimized for PrestaShop importation. If you need a sample file you can learn from, use the ones you can download from the "Download sample CSV files".

The first row should be a descriptive name for the data column (you will be able to skip it during the import process). There must be the same number of columns on each row.

You should remember that:

* The price column will use your store's default currency.
* Categories are to be specified using their existing IDs (so you should have imported them first), and separated with a comma (by default).
* The URL of the image must be an absolute link. In other words, it should be the link that may be used in a web browser in order to display the image. For instance: [http://www.myprestashop/images/productXXX.gif](http://www.myprestashop/images/productXXX.gif).
* The file's character encoding should be UTF-8. If not, use ISO-8859-1.
* Dates use the ISO 8601 format, without a time zone designator (the time zone is the one for your store): `2013-06-21 15:07:27`.

## Uploading the file <a href="#import-uploadingthefile" id="import-uploadingthefile"></a>

Once you have all your data in CSV format, you can upload them to your store's database using the form on this page.

You have two ways to register files to import:

* Using your browser: click the "Upload" button, find your file then validate. Do this as many times as necessary to list all your import files.
* Using your FTP client: upload the files in the `/admin-dev/import` folder of your PrestaShop installation. Reload the import page: the "Choose from history / FTP" button should now indicate a number. Click the button to display the list of available files (including the ones you previously uploaded using the browser), then click the "Use" button for the file you wish to import.

Once your files are all listed in the "Select a file to import" section, you can proceed with the rest of the form:

1. **Confirm the type of data contained in your file**, using the drop-down list named "What do you want to import?". Once you have selected the type of data, the list of the available fields appears on the right, which helps you refine your CSV file – at least for the order of the columns, which will soon prove handy.
2. **Select the language of the imported content**. If the target language is not available, you must install it first, in the "Translations" page under the "International" menu.
3. **Select the separators**. We suggest that you leave the default values ("field separator" with a semicolon "`;`", "multiple value separators" with a comma "`,`"). But obviously, if your CSV file is built differently, you should change these values accordingly.
4. If you want to remove all the products in your catalog before importing, select the appropriate option.
5. Once all your choices have been made, click "Next step".

All import files are uploaded directly in the admin folder's `/import` sub-folder. If the file drop-down menu gets too crowded, you can delete old imports directly using your FTP client.

When clicking the "Next step" button, the page reloads with the data mapping tool. This interface helps you map your file's data columns with the ones required by PrestaShop.

![](<../../../.gitbook/assets/45580390 (4) (4).png>)

Presented in this table are the rows from your file, placed under arbitrary columns matched to PrestaShop's database needs. It is up to you to make sure that all the columns from your CSV file are matched with the correct column header, using each header's drop-down selector, so as to import your content correctly.

For instance, with our sample file:

* **First column**. We marked it as "Enabled", PrestaShop presents "ID" as a header. Click on the header's drop-down menu, and select "Active (0/1)".
* **Second column**. Marked "Name", header indicates "Active (0/1)". Let's change the header for "Name \*".
* **Third column**. You get the idea...

The screen cannot contain more than 6 columns, so click the ">" and "<" buttons to see the other columns, and make sure to match them all correctly.

In our example, we used the first row for column names. Since we do not want these imported, enter "1" in the "Rows to skip" text-field.

Once you are done matching your columns, click the "Import" button (bottom right-hand corner of the screen), and PrestaShop will start the importing process. A pop-up window will open to show you the progress of the import.

When the process is done, it should indicate "100% validated" and "100% imported". When closing this pop-up, you are sent to the main screen. If an error occurred during the import, you will see a notice of all the encountered problems. In this second case, you should review your file and make sure to correct everything.

### Mapping configurations <a href="#import-mappingconfigurations" id="import-mappingconfigurations"></a>

The mapping process can be a tedious task if you cannot customize your file columns order according to that used by the PrestaShop importer, and even more so if you have to do that repeatedly or frequently. That is why PrestaShop includes a small tool to save the current mapping order that you have set up using all the headers drop-down selectors.

![](<../../../.gitbook/assets/23789871 (1) (4).png>)

The tool is a simple field at the top of the matching tool. You can do the three basic actions (only one if there is no mapping configuration saved yet):

* **Saving**. Enter a descriptive name in the field, and click "Save". The interface updates to feature the saved configuration in its drop-down list.
* **Loading**. Select a mapping configuration in the drop-down list, and click "Load".
* **Deleting**. Select a mapping configuration in the drop-down list, and click "Delete".

### Importing Features using Excel <a href="#import-importingfeaturesusingexcel" id="import-importingfeaturesusingexcel"></a>

Excel import is special in that you cannot set the field or multiple value delimiters. Because of that, special attention needs to be paid to “irregular” fields (i.e. fields which are not straightforward text fields and which have several variables). The Features field/column in the Product Import is one of these irregular fields.

The format for Feature column is divided into 4 “parts” each separated by a colon: **featurename:value:position:customizedvalue**

To add multiple features, separate the feature “bundles” by commas e.g. **featurename1:value1:position1:customizedvalue2,featurename2:value2:position2:customizedvalue2,featurename3:value3:position3:customizedvalue3** etc.

Spaces are allowed in each “part” but you cannot use a colon (:) or commas (,) as they are the part and value delimiters respectively and will always be interpreted as so.You can have empty parts for example if you want to keep the “value” part empty. Simply use two colons to skip the part. E.g. Date of Origin::1:1

The description of each part is as follows:

**featurename:** The name of the feature. If this is a selectable (non-customized) value it must be exactly as it appears under Catalog > Features. E.g. Ingredients\


**value**: The value of the feature. If this is a non-customized value, it should be one of the existing values in Catalog > Features otherwise Prestashop will add those values to the list of values.

**position:** The display position of the feature relative to other features, starting at 1.\


**customizedvalue:** 1 (for yes) or 0 (for no). A customized value is one which is not selectable from a list of predefined values in the Catalog > Features screen. Use 0 if you have defined a list of selectable values in the backend.

If you set customizedvalue to 0 and enter a featurename or a value that does NOT exist, the feature and/or value will be added for you.

If you are importing a file which is NOT your default language (i.e. a translation file) then do not include any pre-defined features (i.e. customizedvalue is 0) as this will create a new duplicate feature. The translations for pre-defined features should be done once in the backend via Catalog > Features. For non-default languages add only customized value features.

\
_Also written with the precious contribution of Fadi H. Rezq_\
\
