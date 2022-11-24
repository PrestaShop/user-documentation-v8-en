# Installing PrestaShop on your computer

You may wish to install PrestaShop on your local machine, either in order to test it before investing money in a server and domain name, or to customize your store locally before you push your modifications to the PrestaShop installation that you may already have online.

Installing any web application locally requires that you first install the adequate environment, namely the Apache web server, the PHP language interpreter, the MySQL database server, and ideally the phpMyAdmin tool. This is known as an AMP: Apache+MySQL+PHP. It exists for many operating systems, which provides another letter for the acronym: WAMP (Windows+Apache+MySQL+PHP), MAMP (Mac OS X+...) and LAMP (Linux+...).

## Choosing an AMP package <a href="#installingprestashoponyourcomputer-choosinganamppackage" id="installingprestashoponyourcomputer-choosinganamppackage"></a>

This would require you to be quite technical; luckily there exist many pre-built packages that you can install easily. It does not prevent you from having to get technical here and there, but they do provide a huge help. Since all of the items packaged are open-source, these installers are most of the time free. Here is a selection of free AMP installers:

* EasyPHP: [http://www.easyphp.org/](http://www.easyphp.org/) (Windows)
* MAMP: [http://www.mamp.info/](http://www.mamp.info/) (Mac OS X)
* WampServer: [http://www.wampserver.com/en/](http://www.wampserver.com/en/) (Windows)
* XAMPP: [http://www.apachefriends.org/en/xampp.html](http://www.apachefriends.org/en/xampp.html) (Windows, Mac OS X, Linux, Solaris)

Choose the package that you feel the most comfortable with, and launch it.

## Checking that everything works <a href="#installingprestashoponyourcomputer-checkingthateverythingworks" id="installingprestashoponyourcomputer-checkingthateverythingworks"></a>

Before going on with this PrestaShop installation tutorial, make sure that all the components of your AMP package do work:

*   **The web server should be up and running**. You should be able to access it through your browser, by typing "127.0.0.1" in the address bar.

    [`http://127.0.0.1`](http://127.0.0.1/) is the "localhost", meaning "your computer": it is a loopback address which directs the browser to your local web server.\
    In effect, [`http://127.0.0.1`](http://127.0.0.1/) and [`http://localhost`](http://localhost/) are synonymous: you can use one or the other interchangeably, both send you to the root folder of your local web server.

    Some web servers might not be able to start because their connexion ports (typically, port 80) are already used by another application.

    This often happens when Skype is used. To stop Skype from preventing your local web server to run, go into the Skype advanced settings (Tools > Options > Advanced > Connections) and uncheck the "Use port 80 and 443 as alternatives" option. Restart Skype, and start your local web server again.
* **The database server should be up and running**. MySQL is where all of PrestaShop's data is stored. The AMP package should provide you with a clear indicator whether MySQL is running or not.
* **The phpMyAdmin tool should be accessible**. This is the web application that helps you handle data stored in MySQL. Its location depends on which AMP packaging you chose: it can be found at [`http://127.0.0.1/phpmyadmin`](http://127.0.0.1/phpmyadmin) (XAMPP, WampServer, MAMP), [`http://127.0.0.1/mysql`](http://127.0.0.1/mysql) (EasyPHP), or maybe at another location. Check your package's documentation – it might even provide a phpMyAdmin button that would open the correct URL in your browser.

## Finding the root folder of the local web server <a href="#installingprestashoponyourcomputer-findingtherootfolderofthelocalwebserver" id="installingprestashoponyourcomputer-findingtherootfolderofthelocalwebserver"></a>

Once you have checked that the package is correctly installed and that all of its parts are running, you need to find the root folder of your local web server.

That is the local folder where you will place your application's files, and can be compared to the root folder of your online server, only its content is accessed with [`http://127.0.0.1`](http://127.0.0.1/).

The actual local location of the folder depends greatly on the AMP package, and can be customized:

* EasyPHP: `C:\easyphp\www`
* MAMP: `/Applications/MAMP/htdocs/`
* WampServer: `C:\wamp\www`
* XAMPP: `C:\xampp\htdocs` or `/Applications/xampp/htdocs`

## Finding the MySQL user information <a href="#installingprestashoponyourcomputer-findingthemysqluserinformation" id="installingprestashoponyourcomputer-findingthemysqluserinformation"></a>

Finally, you need to know the root username and password for MySQL, in order to install PrestaShop.

**Most packages use the username "root" with an empty password**, including EasyPHP, MAMP, WampServer and XAMPP.

Read your package's documentation.

## Final note before the installation tutorial <a href="#installingprestashoponyourcomputer-finalnotebeforetheinstallationtutorial" id="installingprestashoponyourcomputer-finalnotebeforetheinstallationtutorial"></a>

With all that clear and done, you can follow up on the rest of this Getting Started guide and start installing PrestaShop.

When you install PrestaShop locally, keep in mind that:

* Files are not to be uploaded via an FTP software (such as Filezilla) to a web server: simply move them in the correct local folder, as indicated above.
* You do not have to create a local domain name: PrestaShop is available through the loopback address indicated above, which is either [`http://localhost`](http://localhost/) or [`http://127.0.0.1`](http://127.0.0.1/) . PrestaShop itself is available at this address by adding its folder's name, for instance [`http://localhost/prestashop`](http://localhost/prestashop) or [`http://127.0.0.1/prestashop`](http://127.0.0.1/prestashop) if PrestaShop is in the `/prestashop/` subfolder of the local root folder. When accessing this address for the first time, you should be automatically redirected to PrestaShop's install, at either [`http://localhost/prestashop/install`](http://localhost/prestashop/install) or [`http://127.0.0.1/prestashop/install`](http://127.0.0.1/prestashop/install) .\


Have you read everything? Now follow the regular installation guide, starting directly at the "Creating a database for your shop" section: [Installing PrestaShop](installing-prestashop.md).
