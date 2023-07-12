# Misc. information

## Keep a test version at hand!

{% hint style="info" %}
Right after you have completed setting up your store, but just before officially opening it to the public, we **strongly** recommend that you install a local test version on your personal computer (using [WAMP](http://en.wikipedia.org/wiki/Comparison\_of\_WAMPs) for Windows, [MAMP](http://en.wikipedia.org/wiki/MAMP) for Mac, or [LAMP](http://en.wikipedia.org/wiki/LAMP\_\(software\_bundle) for Linux, or [XAMPP](http://www.apachefriends.org/en/xampp.html) for any of those platforms), or elsewhere on your hosting server.
{% endhint %}

This second instance will be useful as a pre-production environment in which you can carry out all future changes to your PrestaShop store without affecting the live version. This way, if an error occurs, your live store remains intact and untouched.

After you have confirmed that your test version works as it should, copy the test version over to the live version. It is best to do this after peak usage hours, and with your store properly and temporarily disabled from within the PrestaShop back office.&#x20;

To do so, you can use [Maintenance ](../user-guide/configuring-shop/shop-parameters/general-settings/maintenance.md)mode.

## Checking for the GD library

The [GD library](http://www.boutell.com/gd/) enables PrestaShop to rework images that you upload, especially resizing them.

On a default installation of PHP, the GD Library should be turned on, but if that's not the case for your installation, here are the standard Windows instructions:

1. In the root directory of your PHP folder, **open the `php.ini` file.**
2. **Uncomment the `extension=php_gd2.dll` line** by deleting the ";" at the start of the line. This line should be located about halfway through the file, in the middle of a long list of extensions.
3. **Restart the PHP services**.

{% hint style="info" %}
If you have no access to the `php.ini` file (which is often the case in shared hosting), contact your host about your hosting needs.
{% endhint %}

## Activating PHP 7.2+

{% hint style="warning" %}
To install PrestaShop 8, **PHP 7.2 must be activated.**&#x20;

It is extended to PHP 8.1, but don't attempt to run PrestaShop using PHP 8.2, it won't work.
{% endhint %}

Please do not hesitate to post a bug report concerning the tips needed to make PrestaShop run on your hosting service, on [GitHub](https://github.com/PrestaShop) (you will need an account). We will add them to this guide as we receive them.

The following is a list of procedures of which we are currently aware of.

### 1&1 IONOS

Add this line to your `.htaccess` file:

```
AddType x-mapp-php5 .php
```

For **URL re-writing**, add these lines:

```
Options +FollowSymLinks
RewriteEngine On
```

### Free.fr

Add this line to your `.htaccess` file:

```
php 1
```

### OVH

Add this line to your `.htaccess` file:

```
SetEnv PHP_VER 5
```

To **deactivate global registers**:

```
SetEnv REGISTER_GLOBALS 0
```

### GoDaddy

To **view** your PHP version:

1. Log in to your **Account Manager.**
2. From the Products section, click **Web Hosting.**
3. Next to the hosting account you want to use, click **Launch.**

In the Server section, your PHP Version displays.

To **change** your PHP version:

1. From the **Content** menu, select **Programming Languages.**
2. Select the **PHP version** you want to use, and then click **Continue.**
3. Click **Update**.

{% hint style="info" %}
Changes can take up to 24 hours to complete.
{% endhint %}

### Lunarpages shared hosting

1. Enter **cPanel**. It should be located at [http://www.(your\_domain).(com/net/org/etc)/cpanel](http://www.\(your\_domain\).\(com/net/org/etc\)/cpanel)
2. Enter your **account username and password** in the box that appears.
3. A new page appears. Go to the bottom row of icons on the page and click the icon titled **"Enable/Disable PHP 7.2+"**
4. A new page appears. Click **"Add PHP 7.2+ To Your Account!"**.

{% hint style="info" %}
Your language change request is now submitted! Please allow up to 24 hours for the change to be processed by the hosting server.
{% endhint %}
