# Sample Usages and Specifics

## Data exchange between stores <a href="#sampleusagesandspecifics-dataexchangebetweenstores" id="sampleusagesandspecifics-dataexchangebetweenstores"></a>

### Sharing products and categories <a href="#sampleusagesandspecifics-sharingproductsandcategories" id="sampleusagesandspecifics-sharingproductsandcategories"></a>

When you create a new store within a group, you can choose to have all - or some of - the categories in the new store to be exact duplicates of the categories in any other store on your installation of PrestaShop.

When creating a category, either for a specific store or for all the stores in the PrestaShop installation, PrestaShop registers the category for all the stores – it is simply hidden from any store where it has not been set.

By associating the new stores with a given category, any change in this category will impact all the stores which are associated with it, even if the stores are from different store groups.&#x20;

You can, therefore, change the category's content once and for all from one place, including its products.

**Categories**: A product can only appear in a given category of a store if it has been associated with this category in that store's context. In other words: if store A and store B have the C category in common, you can associate the P product to the C category for the A store's context; and product P will not appear in category C in store B:

<figure><img src="../../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure>

**Carriers**: You can manage the carriers' association on a per-store basis, a per-store-group basis or for all stores; but you cannot customize a carrier on a per-store basis. You must duplicate the carrier if you want to use the same carrier with different price ranges on two stores.

### Sharing customers and customer groups <a href="#sampleusagesandspecifics-sharingcustomersandcustomergroups" id="sampleusagesandspecifics-sharingcustomersandcustomergroups"></a>

As indicated above, stores within the same store group can share clients: all you have to do it set the proper option when creating the store group.

If you want to have different customer groups for each store, you must create a new group and use the "Multistore configuration for" selector to associate the group with the current store or store group.

If the option "Share customers" has been disabled, then your customer list will need to be empty before you can enable this.

If you'd rather keep your customer list you can do the following:

* **Go to your database management software** such as phpMyAdmin.
* **Search for the table** `ps_customer`. It might be different, depending on your database prefix.
* **Export** this table.
* **Empty the table. Do NOT drop it.** If you do want to drop it, make sure you recreate the table afterward.
* **Go back to the multistore settings** for the store group.
* Enable the **"Share customers"** option.
* **Import the table.**

Sharing customers between the store group has now been enabled without the loss of customer information.

### Using a different theme for each store/store group <a href="#sampleusagesandspecifics-usingadifferentthemeforeachshop-shopgroup" id="sampleusagesandspecifics-usingadifferentthemeforeachshop-shopgroup"></a>

Once a theme is installed on your PrestaShop, you can use the "Theme & Logo" page in the "Design" menu to change the theme of the current store, or of the current store group, depending on the context selected in the drop-down selector or the header.

## Using specific settings for each store or group of stores.

If you want your modifications to be applied to a store, a group of stores, or a specific store, check out the "Multistore configuration for" drop-down selector. This is the first element to have a look at when the back office loads: PrestaShop will display different available settings depending on the context in which you are (store, group of stores, all stores).

This allows you to:

* Use a different image format for each store/store group
* Enable/Configure modules for each store
* Display and move blocks in each store's front office
* And a lot more...!

## Managing pages in multistore mode <a href="#sampleusagesandspecifics-managingpagesinmultistoremode" id="sampleusagesandspecifics-managingpagesinmultistoremode"></a>

When viewing the list of content pages in the "All stores" context, all the pages from all stores are displayed. Likewise, when in a store group context, the pages for all the stores in that group are displayed.

When creating a page in a store group context, all the stores in this group will display this page, yet the page will be unique: editing it in one store will apply the changes in all the stores from this group.\
On the creation page, a section appears with a list, indicating which ones will be impacted.

## Managing discounts in multistore mode <a href="#sampleusagesandspecifics-managingdiscountsinmultistoremode" id="sampleusagesandspecifics-managingdiscountsinmultistoremode"></a>

When creating cart rules or catalog price rules in a multistore context, an additional condition is available, with which you can choose the stores on which the rule should be available.

## Webservice and multistore <a href="#sampleusagesandspecifics-web-serviceandmultistore" id="sampleusagesandspecifics-web-serviceandmultistore"></a>

Access to the webservice is also highly configurable, both at the store level and at the store group level. When creating a web-service key, you can choose to associate it with all stores, some store groups, or selected stores.
