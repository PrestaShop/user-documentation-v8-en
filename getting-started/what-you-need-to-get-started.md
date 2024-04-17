---
description: This page lists everything you need to start installing PrestaShop 8.
---

# What you need to get started

## Quick set-up instructions

Here is a quick list of what you need to get started with the installation of PrestaShop 8. You will find more detailed instructions in the next sections.

## **System requirements:**

* **System:** Unix, Linux, or Windows.
* **MySQL:** 5.6 or later.
* **PHP:** 7.2 or later.
* **In your `php.ini` file:**
  * **Useful settings**&#x20;
    * `allow_url_fopen` set to **"On" ✅**,&#x20;
      * `register_globals` set to **"Off" ❌**,
      * `upload_max_filesize` set to **"16MB"** or more.
  * **Must have PHP extensions:**&#x20;
    * **CURL:** the [Client URL extension](https://php.net/manual/en/book.curl.php) is used to download remote resources like modules and localization packages.
    * &#x20;**DOM:** the [DOM extension](https://php.net/manual/en/book.dom.php) is needed to parse XML documents.
    * **Fileinfo:** the [File information extension](https://php.net/manual/en/book.fileinfo.php) is used to find out the file type of uploaded files.
    * **GD:** the [GD extension](https://php.net/manual/en/book.image.php) is used to create thumbnails for the images that you upload.
    * **Intl:** the [ICONV extension](https://www.php.net/manual/en/book.iconv.php) is used to convert character sets.
    * **Mbstring:** the [Multibyte string extension](https://www.php.net/manual/en/book.mbstring.php) is used to perform string operations everywhere.
    * **Zip:** the [Zip extension](https://php.net/manual/en/book.zip.php) is used to expand compressed files such as modules and localization packages.
    * **JSON:** the [JSON extension](https://www.php.net/manual/en/json.installation.php) is used to manage JSON format.
    * **Iconv:** the [ICONV extension](https://www.php.net/manual/en/book.iconv.php) is used to convert character sets.
* **Useful server tools:**&#x20;
  * Cron/[Crontab](https://crontab.guru/), [Memcached](https://memcached.org/).

## Recommended requirements:

* **Hosting:** Unix or Linux.
* **Web server:** Apache Web Server 2.4 (or any later version), or Nginx 1.0 (or later). Note that Apache 2.2 is compatible, but **not recommended** as it [reached its EOL in 2018](https://httpd.apache.org/)[.](https://httpd.apache.org/)
* **Apache module settings are set as:**
  * `mod_rewrite` **enabled ✅**,&#x20;
  * `mod_security` **disabled ❌**,
  * `mod_auth_basic` **enabled ✅**.
* **Server RAM:** At least 256MB of RAM is dedicated to PHP. The more the better.
* **Access codes** to your FTP server and MySQL database. These should be provided by your [web host](what-you-need-to-get-started.md#finding-a-host) if you are not doing a local installation.
* **Text editor:** Any
* **FTP client:** Any
* **Web browser:** Any modern Web browser (if using Internet Explorer: at least IE9).

You also need to know which URL on your domain you want your store(s) to be accessible from.

Once your set-up is in place, you can use the installation guide, available here:

{% content-ref url="installing-prestashop.md" %}
[installing-prestashop.md](installing-prestashop.md)
{% endcontent-ref %}

## Detailed set-up instructions

PrestaShop is a web application. This means it needs to be installed on a web server to run, and that it needs a domain name that your visitors will use to access your store.

## Registering a domain name

Before downloading or installing anything, you **need to provide a home for your PrestaShop online store**.&#x20;

That is made of two components: a **domain name**, and a **web server**.&#x20;

### What's a domain name?

A domain is the online identifier of your website, such as [`example.com`](http://example.com), [`myonlinestore.net` ](http://myonlineshop.net)or [`agreatbrand.store`](https://agreatbrand.store/). It is the **public face of your web server, and therefore, of your store.**

You need to **buy a domain name for your store.** Some web hosting services might provide you with a domain name as many hosts offer a free domain with every new account. They might be free for a year, or for as long as you are a client of that web host. This makes it easier for you to get the full package (hosting + domain name) in one go.

There can be an issue with host-provided domain names: if you find yourself not satisfied with the host's service, you will want to switch to a better host. **This means moving your files, data, and domain name to that other host.**

The files and data are easy to move, but depending on the host, you might have a hard time getting your domain name back.&#x20;

Since your host bought the domain name for you, **technically the domain belongs to them**, and they can **either forbid you to transfer it to another host or make you pay for it.** Since the domain name is your brand, and your address on the web, **you must obey the web host's rules.**

That is why it is often recommended to get your domain name from an independent domain name registrar (see: [http://en.wikipedia.org/wiki/Domain\_name\_registrar](http://en.wikipedia.org/wiki/Domain\_name\_registrar)).&#x20;

{% hint style="warning" %}
Technically, **you can never buy a domain name; you can only rent it**, most of the time for a yearly fee. This gives you the right to use that domain name.&#x20;

**However, as soon as you stop paying for it, it is not yours anymore and anyone can grab it.**
{% endhint %}

In addition to paying for the domain name registration, you will also have to pay for web hosting. You remain free to move to a better host at any time, for no supplementary fee: you have to change the domain name’s DNS addresses. Within 24 hours, the change will spread worldwide.

{% hint style="info" %}
If you would instead get your domain name from an independent registrar, here are some that you can trust:

* **Gandi:** [http://en.gandi.net](http://en.gandi.net/)
* **Namecheap:** [http://www.namecheap.com](http://www.namecheap.com/)
* **GoDaddy:** [https://www.godaddy.com](https://www.godaddy.com/)
* **IONOS:** [https://www.ionos.com](https://www.ionos.com/)
{% endhint %}

### Finding a host

Now that you have a domain name, you **need to have it lead to PrestaShop**. This means that the PrestaShop files need to reside on a web server. You might have a web server of your own, but it is more likely that you have or will have your store hosted by an [Internet hosting service](https://en.wikipedia.org/wiki/Internet\_hosting\_service), which provides you with an online home for a monthly or yearly fee.

Before starting an online store, you will first need to **select a hosting provider**. Just about every web host can effectively handle the PrestaShop solution. However, **only a few hosting providers offer optimized servers for PrestaShop** (with 1-click install and an up-to-date version).&#x20;

You can find the list of the PrestaShop hosting partners [here](https://prestashop.com/prestashop-partners/?taxo\_category\_partner=hosting).

{% hint style="info" %}
When choosing your host, remember **it must provide you with support for:**

* **PHP 7.2+**, which is the programming language with which PrestaShop is written,&#x20;
* **MySQL 5.6+**, which is the database system where PrestaShop stores all its data.&#x20;

Note that there are more requirements. see the **"Technical requirements"** section below.
{% endhint %}

### Technical requirements

PrestaShop is an application that runs on a web server and uses the PHP programming language. **It stores its data in a MySQL server.**

[PHP](https://www.php.net/) is an open-source **programming language**, mainly used for web applications. Created in 1995, it has since become the most used programming language by web developers. It uses a C-like syntax, making it easy to learn.

[MySQL](https://www.mysql.com/) is an open-source **database management system**. Also created in 1995, it's become the most used database system by web developers. It is based on the SQL language, the most widely used database language.

No matter which hosting service you choose, **the following components will be installed on your web server:**

* **System**: Unix, Linux, or Windows (Unix is highly recommended).
* **Web server**: Apache Web server 2.2 or later.
* **PHP:** 7.2 or later.&#x20;
* **MySQL:** 5.6 or later.
* **Server RAM:** At least `256MB`of RAM.

{% hint style="info" %}
PrestaShop can also work with [Microsoft's IIS Web server](https://www.iis.net/) 6.0 or later, and [Nginx](https://docs.nginx.com/nginx/admin-guide/web-server/) 1.0 or later.
{% endhint %}

## Tools

You will need two tools:&#x20;

* **a text editor** to edit text files,
* **an FTP client** to transfer files from your machine to your server and vice-versa.

### **Text editor**

Here are some well-known text editors, feel free to use whichever best suits your needs:

* **Windows:**
  * Sublime Text: [http://www.sublimetext.com/](http://www.sublimetext.com/)
  *
* **MacOS :**
  * Sublime Text: [http://www.sublimetext.com/](http://www.sublimetext.com/)
  * BBEdit: [https://www.barebones.com/products/bbedit/](https://www.barebones.com/products/bbedit/)
* **Unix/Linux:**
  * Vim: [http://www.vim.org/](http://www.vim.org/)
  * Emacs: [http://www.gnu.org/software/emacs/](http://www.gnu.org/software/emacs/)

{% hint style="warning" %}
**Do not use a word processor** such as Microsoft Word or [OpenOffice](http://openoffice.org) Writer when editing text files.
{% endhint %}

### **FTP client**

**FTP** is short for "File Transfer Protocol", which is the standard way used to transfer files from a computer to a web host.

#### Using Filezilla

In this guide, we will use **Filezilla**, which is a great and free FTP client for Windows, MacOS, and Linux.&#x20;

{% hint style="info" %}
**Download FileZilla** from [http://filezilla-project.org/](http://filezilla-project.org/) and **install it.**&#x20;

Do not download FileZilla Server, only **FileZilla Client**!
{% endhint %}

Once FileZilla is installed, you will need to **configure it** with the connection parameters of your web server. Your host should have sent you these parameters. If not, ask them! Make sure to check your spam folder.

You'll need these parameters:

* **a hostname** or **an IP address**: the location of your hosting space's FTP server.
* **a username**: your hosting account identifier, which is unique to you.
* **a password**: a compulsory security measure.

**Open** FileZilla, and open the **Site Manager tool**. You can do this in three different ways:

* Press **Ctrl+S**,
* Click the **"Open the Site Manager" icon**, at the top left corner,
* Open the **"File" menu**, and select the **"Site Manager" option.**

A window opens:

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption><p>FileZilla's Site Manager page.</p></figcaption></figure>

To **add your hosting space** to the Site Manager:

1. Click the **"New Site"** button. A new entry is created in the site list. Give it a recognizable name.
2. On the right side, in the **"General"** tab, enter the parameters your host provided you with (**Host**, **User**, and **Password**). You should not have to change the other default parameters unless your host tells you otherwise.
3. Once all the fields are properly filled, click the **"Connect"** button. This will save your site in the list and log you into your account so that you can make sure everything works right.

{% hint style="info" %}
If FileZilla does not suit you, here are a few other well-known FTP clients:

* **Windows:**
  * CoreFTP: [http://www.coreftp.com/](http://www.coreftp.com/)
  * WinSCP: [http://winscp.net/](http://winscp.net/)
  * SmartFTP: [http://www.smartftp.com/](http://www.smartftp.com/)
* **Mac OS:**
  * Cyberduck: [http://cyberduck.ch/](http://cyberduck.ch/)
  * Transmit: [http://www.panic.com/transmit/](http://www.panic.com/transmit/)
  * Fetch: [http://fetchsoftworks.com/fetch/](http://fetchsoftworks.com/fetch/)
* **Unix/Linux:**
  * gFTP: [http://gftp.seul.org/](http://gftp.seul.org/)
  * NcFTP: [http://www.ncftp.com/ncftp/](http://www.ncftp.com/ncftp/)
  * Kasablanca: [http://kasablanca.berlios.de/](http://kasablanca.berlios.de/)
{% endhint %}

## Making a plan

**You should decide right away where you want to host PrestaShop.**&#x20;

There are four possibilities relating to your domain name:

* At the **root of the domain**: [http://www.example.com/](http://www.example.com/)
* In a **folder**: [http://www.example.com/shop/](http://www.example.com/shop/)
* In a **sub-domain**: [http://store.example.com/](http://store.example.com/)
* In a **folder of a sub-domain**: [http://clothes.example.com/boutique/](http://clothes.example.com/boutique/)

{% hint style="success" %}
Thanks to the [multistore feature](../user-guide/configuring-shop/advanced-parameters/multistore.md), you can have as many stores as necessary with a single installation of PrestaShop 8, each with its own specific domain name if necessary. You should take that into account when deciding what goes where.

Whatever your plan is, the default store will always reside where PrestaShop itself is located.
{% endhint %}

## Installing PrestaShop

Now that all the requirements are in place, you're ready to begin installing PrestaShop!&#x20;

**➡️ Check out the installation guide here:**&#x20;

{% content-ref url="installing-prestashop.md" %}
[installing-prestashop.md](installing-prestashop.md)
{% endcontent-ref %}



{% hint style="success" %}
_This page has been recently updated!_

**🗣 What did you think of this article? Let us know!**&#x20;

Your feedback helps us improve PrestaShop's documentation for everyone! 🙌

You can use the emojis on the bottom right of this article to let us know what you think about this article ⬇️
{% endhint %}
