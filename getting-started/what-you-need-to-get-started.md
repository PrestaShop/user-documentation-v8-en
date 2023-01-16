# What you need to get started

## Quick set-up instructions

Here is a quick list of what you need to get started with the installation of PrestaShop V.8. Should you not feel comfortable with the lack of details, you will find detailed instructions in the sections following this one.

* System requirements:
  * PHP 7.1 or later.
    * Useful settings (in the `php.ini` file): \

      * `allow_url_fopen` set to On,&#x20;
      * `register_globals` set to Off`,`
      * `upload_max_filesize` set to "16M" (or more).
    * Must-have PHP extensions (in the `php.ini` file): CURL, DOM, Fileinfo, GD, Intl, Mbstring, Zip, JSON, Iconv.
    * Useful server tools: cron/crontab, Memcached.
  * MySQL 5.6 or later.
  * Better if: \

    * Unix/Linux hosting.
    * Apache Web Server 2.2 or later or nginx Web Server.
      * Apache module settings:&#x20;
        * `mod_rewrite` enabled,&#x20;
        * `mod_security` disabled,
        * `mod_auth_basic` enabled.
    * At least 256 Mb of RAM is dedicated to PHP. The more the better.
* Access codes to your FTP server, your MySQL database
  * These should be provided by your web host if you are not doing a local installation.
* Any text editor.
* Any FTP client.
* Any modern Web browser (if using Internet Explorer: at least IE9).

You also need to know which URL on your domain you want your store(s) to be accessible from.

Check the official system requirements page: [http://www.prestashop.com/en/system-requirements](http://www.prestashop.com/en/system-requirements).

Once your set-up is in place, you can use the installation guide:&#x20;

{% content-ref url="installing-prestashop.md" %}
[installing-prestashop.md](installing-prestashop.md)
{% endcontent-ref %}

## Detailed set-up instructions

PrestaShop is a web application: it needs to be installed on a web server in order to run, and it needs a domain name that your visitors will use to access your store.

### Registering a domain name

Before downloading or installing anything, you need to provide a home for your PrestaShop online store. That is made of two components: a domain name, and a web server. A domain is the online identifier for your website, such as [`example.com`](http://example.com), [`myonlineshop.net` ](http://myonlineshop.net)or [`agreatbrand.store`](https://agreatbrand.store/). It is the public face of your web server, and therefore of your store.

You need to buy a domain name for your store. You might get one when you get your web hosting in place: many web hosts offer a free domain with every new account. They might be free for a year, or for as long as you are a client of that web host. This makes it easy to get the full package (hosting+domain name) in one go. For more information about domains, see the list of independent registrars below or follow the link: [https://www.prestashop.com/en/domain](https://www.prestashop.com/en/domain).

There can be an issue with host-provided domain names: if you find yourself not satisfied with the host's service, you will want to switch to a better host. This means moving your files, data and domain name to that other host.

The files and data are easy to move, but depending on the host, you might have a hard time getting your domain name back. Since they bought the domain name for you, technically the domain belongs to them, and they can either forbid you to transfer it to another host, or they can make you pay for it. And since the domain name is your brand and your address on the web, you must obey the web host's rules.

That is why it is often recommended to get your domain name from an independent domain name registrar (see: [http://en.wikipedia.org/wiki/Domain\_name\_registrar](http://en.wikipedia.org/wiki/Domain\_name\_registrar)). Technically, you can never buy a domain name; you can only rent it, most of the time for a yearly fee. This gives you the right to use that domain name, but as soon as you stop paying for it, it is not yours anymore and anyone can grab it for himself.

In addition to paying for the domain name registration, you will also have to pay for web hosting. But at least you remain free to move to a better host at any time, for no supplementary fee: you just have to change the domain name’s DNS addresses. Within 24 hours, the change will be spread across the world.

If you would rather get your domain name from an independent registrar, here are some that you can trust:

* Gandi: [http://en.gandi.net/](http://en.gandi.net/)
* Namecheap: [http://www.namecheap.com/](http://www.namecheap.com/)
* GoDaddy: [https://www.godaddy.com/](https://www.godaddy.com/)
* 1&1 IONOS: [https://www.ionos.com](https://www.ionos.com/)

There are many more. Ask your friends about them!

### Finding a host

Now that you have a domain name, you need to have it lead to PrestaShop. This means that the PrestaShop files need to reside on a web server. You might have a web server of your own, but it is more likely that you have or will have your store hosted by an Internet hosting service (see: [http://en.wikipedia.org/wiki/Internet\_hosting\_service](http://en.wikipedia.org/wiki/Internet\_hosting\_service)), which provides you with an online home for a monthly or yearly fee.

Before starting an online store, you will first need to select a hosting provider. Just about every web host can effectively handle the PrestaShop solution. However, only a few hosting providers offer optimized servers for PrestaShop (with 1-click install and up-to-date version). Here is our[ list of hosting partners](https://www.prestashop.com/en/ecommerce-hosting).

When choosing your host, remember one crucial requirement: it must provide you with support for PHP 7.1 (or more recent), the programming language with which PrestaShop is written, and MySQL 5.6 (or more recent), the database system where PrestaShop stores all its data. There are more requirements: see the "Technical requirements" section below.

### Technical requirements

PrestaShop is an application which runs on a web server and is written using the PHP programming language. It stores its data in a MySQL server.

PHP is an open-source programming language, mainly used for web applications. Created in 1995, it has since become the most used programming language by web developers. It uses a C-like syntax, making it easy for developers to learn it.

MySQL is an open-source database management system. Also created in 1995, it has since become the most used database system by web developers. It is based on the SQL language, the most widely used database language.

Whichever hosting service you choose, the following components shall be installed on your web server:

* **System**: Unix, Linux, or Windows. Unix is highly recommended.
* **Web server**: Apache Web server 2.2 or later.
* **PHP 7.1 or later**.&#x20;
* **MySQL 5.6 or later**.
* At least 256 Mb of RAM on your server.

PrestaShop can also work with Microsoft's IIS Web server 6.0 or later, and nginx 1.0 or later.

More information is available for system administrators in the [System Administrators Guide](http://doc.prestashop.com/display/PS15/System+Administrator+Guide). Make sure to read it!

### Tools

You will need two tools: a text editor, in order to edit text files, and a FTP client, in order to transfer files from your machine to your server and vice-versa.

**Text editor**

Here are a few well-known text editors:

* Windows and OS X:
  * Sublime Text: [http://www.sublimetext.com/](http://www.sublimetext.com/)
  * Atom: [https://atom.io/](https://atom.io/)
* Unix/Linux:
  * Vim: [http://www.vim.org/](http://www.vim.org/)
  * Emacs: [http://www.gnu.org/software/emacs/](http://www.gnu.org/software/emacs/)

Do NOT use a word processor when editing text files, such as Microsoft Word or [OpenOffice.org](http://openoffice.org)'s Write.

**FTP client**

FTP is short for "File Transfer Protocol", meaning the standard way used to transfer files from a computer to a web host

In this guide, we will use Filezilla, which is a great and free FTP client for Windows, Mac OS X, and Linux. Download it from [http://filezilla-project.org/](http://filezilla-project.org/) and start its installer. Note: do not download FileZilla Server, only FileZilla Client!

Once FileZilla is installed, you will need to configure it with the connection parameters of your web server, which should have been sent to you by your host. If not, ask for them to your host – or check your spam folder.

Basically, the needed parameters are:

* **a hostname** or **an IP address**: the location of your hosting space's FTP server.
* **a username**: your hosting account identifier, which is unique to you.
* **a password**: a compulsory security measure.

Open FileZilla, and open its Site Manager tool. You can do this in three different ways:

* Press Ctrl-S,
* Click the "Open the Site Manager" icon, at the top left corner,
* Open the "File" menu, and select the "Site Manager..." option.

A window opens.

To add your hosting space to the Site Manager:

1. Click the "New Site" button. A new entry is created in the site list. Give it a recognizable name.
2. On the right side, in the "General" tab, enter the parameters your host provided you with: host, user, and password. You should not have to change the other default parameters unless told so by your host.
3. Once all the fields are properly filled, click the "Connect" button. This will both save your site in the list, and log you into your account, so that you can make sure everything works right.

If FileZilla does not suit you, here are a few other well-known FTP clients:

* Windows:
  * CoreFTP: [http://www.coreftp.com/](http://www.coreftp.com/)
  * WinSCP: [http://winscp.net/](http://winscp.net/)
  * SmartFTP: [http://www.smartftp.com/](http://www.smartftp.com/)
* Mac OS X:
  * Cyberduck: [http://cyberduck.ch/](http://cyberduck.ch/)
  * Transmit: [http://www.panic.com/transmit/](http://www.panic.com/transmit/)
  * Fetch: [http://fetchsoftworks.com/fetch/](http://fetchsoftworks.com/fetch/)
* Unix/Linux:
  * gFTP: [http://gftp.seul.org/](http://gftp.seul.org/)
  * kasablanca: [http://kasablanca.berlios.de/](http://kasablanca.berlios.de/)
  * NcFTP: [http://www.ncftp.com/ncftp/](http://www.ncftp.com/ncftp/)

## Making a plan

You should decide right away where you want to host PrestaShop. There are four possibilities relating to your domain name:

* At the root of the domain: [http://www.example.com/](http://www.example.com/)
* In a folder: [http://www.example.com/shop/](http://www.example.com/shop/)
* In a sub-domain: [http://store.example.com/](http://store.example.com/)
* In a folder of a sub-domain: [http://clothes.example.com/boutique/](http://clothes.example.com/boutique/)

Note that thanks to the multistore feature, you can have as many stores as necessary with a single installation of PrestaShop V.8, each with its own specific domain name if necessary. You should take that into account when deciding what goes where.\
Whatever your plan is, the default store will always reside where PrestaShop itself is located.

## Installing PrestaShop

Finally, now that all the requirements are in place, you can use the installation guide:&#x20;

{% content-ref url="installing-prestashop.md" %}
[installing-prestashop.md](installing-prestashop.md)
{% endcontent-ref %}
