# SEO and URLs

The tools on this page help you improve the presence of your PrestaShop site on web searches and therefore reach more potential customers.

SEO means "Search Engine Optimization". It represents a set of techniques and best practices aimed at improving the visibility of a website on search engines. You can read more about this on [Wikipedia](http://en.wikipedia.org/wiki/Search\_engine\_optimization). URL is short for "Uniform Resource Locator" or, simply put, the online address of a web page. You can read more about what a URL is on [Wikipedia](http://en.wikipedia.org/wiki/URL).

By default, PrestaShop's deep URLs (that is, specific pages rather than online the domain name) are uninformative to both customers and search engines: a URL such as [http://www.myprestashop.com/product.php?id\_product=27](http://www.myprestashop.com/product.php?id\_product=27) does not help visitors know what product is on that page. Friendly URLs are the way to achieve that and get for instance [http://www.myprestashop.com/2-music-players/27-ipod-nano-green](http://www.myprestashop.com/2-music-players/27-ipod-nano-green).

As you can see in the second example above, both categories and products can have a friendly URL: in the example above, `id_category=2` becomes `2-music-players`, and `id_product=27` becomes `27-ipod-nano-green`. While the ID number cannot be removed by default, the words can be either generated from the category/product name or written by hand. This is done directly in the configuration page for the product or the category (in the "Catalog" menu): the "Friendly URL" field can be found directly on the main configuration page of a category and under the "SEO" tab of the configuration page of a product.

There are other individual pages in your PrestaShop install that would certainly benefit from friendly URLs: CMS pages, user account pages, pages with automatically generated content. The "SEO & URLs" page presents you with a list of these pages and enables you to edit their friendly URLs as well as their meta tags (title, description, keyword).

![](<../../../../.gitbook/assets/64225659 (4) (4) (3).png>)

Friendly URLs only work with a server setup that supports URL rewriting (through the Apache Web Server `mod_rewrite` feature, for instance). Make sure to check that your server does (if needed, ask your hosting provider!), as it can make your shop completely unavailable to customers if you enable friendly URLs and the server does not support it!

### &#x20;Homepage SEO settings <a href="#seoandurls-homepageseosettings" id="seoandurls-homepageseosettings"></a>

In order to change the homepage meta tags, you simply need to open the "SEO & URLs" page and click on "index" to reach the page's settings and freely edit its important SEO information.

![](../../../../.gitbook/assets/64225660.png)

A few tips:

* The default homepage title is the name of the store, and therefore the index' title field is empty. If you put content in the field, the homepage's full title will be replaced by your input. The name of the store itself is set during the installation of PrestaShop and can be changed from the "Contact Details" tab, available in the Shop Parameters > Contact section of the back office.
* Keep your description short: a paragraph of text is enough.
* To add a meta keyword, click on the field and validate by pressing "Return". You can remove tags by clicking the cross.
* You do not have to add a rewritten URL if there is already one.

Note that if your store has already been indexed by Google or any other search engine, it might take a while for your changes to appear in the search results... you might have to be patient!

## Adding a new friendly URL <a href="#seoandurls-addinganewfriendlyurl" id="seoandurls-addinganewfriendlyurl"></a>

Friendly URLs are to be set in the configuration page of each product, category, or static content page. This creation page is only useful for some automatic pages, and most of the time you won't have to worry about these.

Make sure to fill the fields for all the available languages on your shop: not only is it immensely useful to local users, but some search engines can even make use of this local information.

![](../../../../.gitbook/assets/64225660.png)

Click the "Add new page" button to reach the friendly URL creation form. It has a handful of fields:

* **Page**. The drop-down list gives you all the pages that can benefit from a friendly URL.
* **Page title**. The title that will appear in search engines when a request is made.
* **Meta description**. A presentation of the page in just a few words, intended to capture a customer's interest. It will appear in the search results.
* **Meta keywords**. Keywords that you must define in order to have your site referenced by search engines. You can enter several of them: type the words, press the "Return" key, and see how the tag gets encapsulated in a blue block, with a tiny cross icon to delete it.
* **Rewritten URL**. This is where you set the friendly URL. Make it short and descriptive, use only letters and numbers, and replace spaces (" ") by hyphens ("-").

## Set up URLs <a href="#seoandurls-setupurls" id="seoandurls-setupurls"></a>

The main options for friendly URLs:

*   **Friendly URL**. Change this option _if you know that your server ****_ can support URL rewriting. If not, leave it at "No".

    You may see a message such as "_URL rewriting (mod\_rewrite) is not active on your server or it is not possible to check your server configuration. If you want to use Friendly URLs you must activate this mod_". In this case, PrestaShop cannot detect your server settings, but that does not mean the feature will not work. You must test it yourself.
* **Accented URL**. PrestaShop can produce URL with special characters, for products with non-ASCII names. You can disable that option here.
*   **Redirect to the canonical URL**. A given PrestaShop page can have many URLs, most often when there are parameters to consider: for instance, [`http://example.com/product.php?id=5&option1`](http://example.com/product.php?id=5\&option1) and [`http://example.com/product.php?id=5&option2`](http://example.com/product.php?id=5\&option2) point to the very same product, only one difference. Since you want your product to have a single URL and not many duplicate ones, you should enable canonical URLs.\
    \
    Canonical URLs are a way to eliminate self-created duplicate content – which can dramatically bring your search engine rank down, as this is considered spam. To avoid search engines thinking you are spamming their index, PrestaShop uses standard `rel="canonical"` link tag to indicate which is the one base URL for a given content. While it is highly recommended to enable this option, it also depends on your theme implementing correctly the `<link>` header tag. If needed, ask the theme designer for more information.

    \
    _New since 1.7.6!_ By default, it is the canonical URL of a product that is called and, in case of combinations, the canonical URL points towards the default combination.\
    \
    There are three options:

    * _No redirection._ You might get duplicate URLs.
    * _301 Move Permanently._ Returns the HTTP 301 status code, pointing to the main URL and notifying search engines that this is the only URL to take into account. We recommend this option once your modifications are done.
    * _302 Moved Temporarily._ Returns the HTTP 302 status code, pointing to the main URL and notifying search engines that the main URL might change later.
* **Disable Apache's MultiViews option**. Apache is the most popular webserver and is most likely the one your web host uses for your site (although you should check this for yourself). Multiviews is a content negotiation system: when enabled, the web server tries to serve the user a page in what it thinks is the best matching language version, under the same URL. Unfortunately, this might bring trouble to PrestaShop's friendly URLs feature. If this is the case, you can try to disable multi-views with this option.
* **Disable Apache's mod\_security module**. `mod_security` is a module of the Apache web server, which acts as a firewall, protecting your server from intrusions. It can, however, block some key features, or even produce errors in some configuration. In such case, disable that firewall here.\
  \


![](<../../../../.gitbook/assets/64225661 (4) (4) (3).png>)

## Set shop URL <a href="#seoandurls-setshopurl" id="seoandurls-setshopurl"></a>

In this section, you can view and edit some of the default server settings:

* **Shop domain**. Your store's main domain name or IP address.
* **SSL domain**. Your store's secure domain name (`https://`) or IP address.
* **Base URI**. The folder where you installed PrestaShop. If it is at the root of the domain, use "`/`".

Most of the time, we recommend not to touch these fields without knowing exactly what you are doing. Indeed, a single mistake can sometimes break your shop.

![](<../../../../.gitbook/assets/64225662 (4).png>)

## Schema of URLs <a href="#seoandurls-schemaofurls" id="seoandurls-schemaofurls"></a>

_Is displayed only if friendly URLs are enabled._

You can change the way friendly URLs are generated, by changing the route to a resource in your shop. For instance, the default route to display a product's page is `{category:/}{id}-{rewrite}{-:ean13}.html`, which results in `/summer-dresses/7-printed-chiffon-dress.html`. You could change that route to `{manufacturer:/}{id}-{rewrite:/}` to obtain `/fashion-manufacturer//7-printed-chiffon-dress/`

Eight fields are available by default, and each is accompanied by a list of available keywords. Some keywords are mandatory and are indicated with a "\*".

![](<../../../../.gitbook/assets/64225664 (3) (4).png>)

Once your fields updated, do not forget to save your changes!

## SEO options <a href="#seoandurls-seooptions" id="seoandurls-seooptions"></a>

_New since 1.7.5.1!_ PrestaShop now allows you to enable the display of your product's attributes in its meta title.

![](<../../../../.gitbook/assets/64225663 (2) (1) (3).png>)

## Robots file generation <a href="#seoandurls-robotsfilegeneration" id="seoandurls-robotsfilegeneration"></a>

A `robots.txt` file enables you to block specific automated bots and web spiders which crawl the Web in order to find more web pages to add to their company's servers. Some bots you want to have full access to your website, such as Google's or Yahoo!'s, and some others you would rather not, such as spam bots, content thieves, e-mail collectors, etc. Note that the worst of bots do not respect this file's directives, as it is purely advisory.

PrestaShop's `robots.txt` generation tool simply creates a file with exclusion directives for files and directories that are not meant to be public, and should not be indexed. These directives apply to all bots, good or bad: the generated file uses the "User-agent: \*" string.

Clicking on the "Generate robots.txt" button replaces any existing `robots.txt` file with a new one. Therefore, if you want to add your own rules, do it after PrestaShop has generated its version of the file.

![](<../../../../.gitbook/assets/64225665 (4) (4).png>)

Video - 4 Tips to Well start SEO for your Ecommerce site

[![](<../../../../.gitbook/assets/51839782 (6) (6) (3).png>)](https://www.youtube.com/watch?v=NnPEoE3MuHk\&index=13\&list=PLyZYn1MMU7-xT-L\_zUyGnRBJmAuP6uc-c)
