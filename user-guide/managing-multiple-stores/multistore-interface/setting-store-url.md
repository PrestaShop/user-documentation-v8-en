# Setting a store's URL

## Composition of a store's URL

![](<../../../.gitbook/assets/httpswww.mystore.comwomen (1).png>)

## Having two stores on one domain name

Two stores can't share the same URL.&#x20;

However, you can have as many stores as you want on one domain name by using a sub-folders or sub-domains.

### **Using sub-folders**

![](<../../../.gitbook/assets/httpswww.mystore.comwomen (4).png>)

In the case of subfolder stores, make sure to create 2 URLs for each store: one with the "www.", and one without it.​

Otherwise, customers trying to access your secondary store without the "www." in the URL will be redirected to your main store.

### &#x20;**Using sub-domains**

![](<../../../.gitbook/assets/httpswww.mystore.comwomen (5) (2).png>)

{% hint style="success" %}
You don't have to create subdomains or subfolders manually. PrestaShop will create the path on your server automatically.
{% endhint %}

### Using a different domain name

In case you want to use a different domain name for your supplemental store rather than a subdomain or a subfolder, you must configure your domain to point to the folder where PrestaShop is located. The URL rewriting is then done by PrestaShop itself.

Alternatively, you can create an alias for your domain name that redirects to the absolute URL where your installation of PrestaShop is located. The way to achieve this depends on the control panel and options that your hosting company provides you with: "Alias" for Plesk, "Forward" for CPanel, "Aliasdomain" for ISPConfig, etc.

## Setting a URL&#x20;

To set a URL for a store**:**

1. Select the store in the Multistore tree
2. Click on the link "Click here to set a URL for this shop" in "Main URL" column of the table.
3. Fill in the form&#x20;

**URL options:**

![](<../../../.gitbook/assets/image (51).png>)

* **Shop:** Selected the store on which you want to set the URL.
* **Main URL:** Switch the button to "Yes" if you want all the URLs of the store to redirect to the main URL.
* **Status:** All URLs, expect for the main one, can be disabled.

**Shop URL:**

![](<../../../.gitbook/assets/image (50).png>)

*   **Domain:** Enter the store's domain name. You can indicate a sub-domain if needed. Just make sure it doesn't contain '`http://`', or any '`/`'.&#x20;

    Example: [`www.example.com`](http://www.example.com) or [`kids.example.com`](http://kids.example.com).
* **Domain SSL:** If your SSL domain is different from your main domain, be sure to indicate it in that field.
* **Physical URL:** Enter the physical path of your installation on your server. If you installed the store in the root directory, then the physical URL should be `/`. Alternatively, if you installed your store in a sub-folder, the physical URL is the name of the subfolder.
*   **Virtual URL:** Thanks to URL rewriting, you can use this option if you want to create a store with a URL that doesn't exist on your server, without having to create a sub-folder. For example, if you want your store to be available with the URL `www.example.com/my-store/shoes/`, you have to set `shoes/` in this field, assuming that `my-store/` is your physical URL.&#x20;

    Friendly URLs must be enabled in **Shop Parameters >Traffic & SEO**. Note that this option only works for subfolder stores, not subdomain stores.&#x20;
* **Final URL:** Here, you can get a preview of what the store's URL will look like, based on above settings.&#x20;

