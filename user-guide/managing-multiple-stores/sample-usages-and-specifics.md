# Sample Usages and Specifics

## Data exchange between stores <a href="#sampleusagesandspecifics-dataexchangebetweenstores" id="sampleusagesandspecifics-dataexchangebetweenstores"></a>

### Sharing products and categories <a href="#sampleusagesandspecifics-sharingproductsandcategories" id="sampleusagesandspecifics-sharingproductsandcategories"></a>

When you create a new store within a group, you can choose to have all, or some, of the categories in the new store to be exact duplicates of the categories in any other store on your installation of PrestaShop.

When creating a category, either for a specific store or for all the stores in the PrestaShop installation, PrestaShop registers the category for all the stores – it is simply hidden from any store where it has not been set.

By associating the new stores with a given category, any change in this category will impact all the stores which are associated with it, even if the stores are from different store groups. You can, therefore, change the category's content once and for all from one place, including its products.

**Categories**: A product can only appear in a given category of a shop if it has been associated with this category in that shop's context. In other words: if shop A and shop B have the C category in common, you can associate the P product to the C category for the A shop's context, and P will not appear in category C on shop B.

**Carriers**: You can manage the carriers' association on a per-shop basis, a per-shop-group basis or for all shops; but you cannot customize a carrier on a per-shop basis. You must duplicate the carrier if you want to use the same carrier with different price ranges on two shops.

### Sharing customers and customer groups <a href="#sampleusagesandspecifics-sharingcustomersandcustomergroups" id="sampleusagesandspecifics-sharingcustomersandcustomergroups"></a>

As indicated above, stores within the same store group can share clients: all you have to do it set the proper option when creating the store group.

If you want to have different customer groups for each store, you must create a new group and use the "Multistore configuration for" selector to associate the group with the current store or store group.

If the option "Share customers" has been disabled, then your customer list will need to be empty before you can enable this.

If you'd rather keep your customer list you can do the following:

* Go to your database management software such as phpMyAdmin.
* Search for the table `ps_customer`. It might be different, depending on your database prefix.
* Export this table.
* Empty the table. Do NOT drop it. If you do want to drop it, make sure you recreate the table afterward.
* Go back to the multistore settings for the shop group.
* Enable the "Share customers" option.
* Import the table.

Sharing customers between the shop group have now been enabled without the loss of customer information.

### Sharing orders <a href="#sampleusagesandspecifics-sharingorders" id="sampleusagesandspecifics-sharingorders"></a>

It is possible for stores within the same store group to share orders: all you have to do it set the proper option when creating the store group.

If the option "Share orders" has been disabled, then your order list will need to be empty before you can enable this.

If you'd rather keep your orders you can do the following:

* Go to your database management software such as phpMyAdmin.
* Search for the table `ps_order`. It might be different, depending on your database prefix.
* Export this table.
* Empty the table. Do NOT drop it. If you do want to drop it, make sure you recreate the table afterward.
* Go back to the multistore settings for the shop group.
* Enable the "Share orders" option.
* Import the table.

Sharing orders between the shop group have now been enabled without the loss of order information.

### Using a different theme for each shop/shop group <a href="#sampleusagesandspecifics-usingadifferentthemeforeachshop-shopgroup" id="sampleusagesandspecifics-usingadifferentthemeforeachshop-shopgroup"></a>

Once a theme is installed on your PrestaShop, you can use the "Theme & Logo" page in the "Design" menu to change the theme of the current store, or of the current store group, depending on the context selected in the drop-down selector or the header.



## Managing pages in multistore mode <a href="#sampleusagesandspecifics-managingpagesinmultistoremode" id="sampleusagesandspecifics-managingpagesinmultistoremode"></a>

When viewing the list of the content pages in the "All shops" context, all the pages from all shops are displayed. Likewise, when in a shop group context, the pages for all the shops in that group are displayed.

When creating a page in a shop group context, all the shops in this group will display this page, yet the page will be unique: editing it in one shop will apply the changes in all the shops from this group.\
On the creation page, a section appears with a list, indicating which ones will be impacted.

## Managing discounts in multistore mode <a href="#sampleusagesandspecifics-managingdiscountsinmultistoremode" id="sampleusagesandspecifics-managingdiscountsinmultistoremode"></a>

When creating cart rules or catalog price rules in a multistore context, an additional condition is available, with which you can choose the shops on which the rule should be available.

## Web-service and multistore <a href="#sampleusagesandspecifics-web-serviceandmultistore" id="sampleusagesandspecifics-web-serviceandmultistore"></a>

Access to the web-service is also highly configurable, both at the shop level and at the shop group level. When creating a web-service key, you can choose to associate it with all shop, some shop groups, or selected shops.
