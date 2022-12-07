# Modules Selection

You can discover and install new modules to improve your store when you’re beginning or growing your activity.

* [Explaining modules and services](modules-selection.md#what-is-the-difference-between-a-module-and-service)
* [Uploading and installing a module manually ](modules-selection.md#modulesselection-uploadingamodulemanually)
  * [Installing using the upload form](modules-selection.md#ModulesSelection-Installingusingtheuploadform)
  * [Installing using an FTP client](modules-selection.md#ModulesSelection-InstallingusinganFTPclient)

### What is the difference between a module and a service?

On the one hand, **a module** allows you to add features to your store, such as new means of payment, a synchronization of inventory and orders with your logistician, an export to smart shopping guides, and many tools for you and your customers. Modules come with a file that must be installed on your store.

On the other hand, **a service** is intangible: you do not have to install anything in your store for the service to work. Instead, you may have to sign a contract with the service provider.

#### **What is a built-in module?**

Built-in (or native) modules are available within your store from its setup. Some modules are already pre-installed to help your store run (you will find them in the "Installed modules" tab), and some you can upload and install manually. You can choose to keep them or not, depending on your needs. They cover the basics of e-commerce and come for free.

## Uploading and  installing a module manually  <a href="#modulesselection-uploadingamodulemanually" id="modulesselection-uploadingamodulemanually"></a>

#### Installing using the upload form <a href="#modulesselection-installingusingtheuploadform" id="modulesselection-installingusingtheuploadform"></a>

To install a new module automatically, click on the "Upload a module" button at the top of the page. A pop-up window will open.

![](<../../../../.gitbook/assets/51185188 (4) (2) (4).png>)

This block enables you to upload the archive file of the module, as downloaded. You can either upload a `zip` file, or a `tar.gz` one (tarball). Simply drop the module's file here, or browse to the file that you downloaded by clicking on "select file". Do not point to the module's uncompressed folder or any of its unpacked files: only the archive file!&#x20;

Once the file is detected, the installation will start automatically: the software will upload the module from your computer to its server, unpack it, place the files in the correct location, and update the page, all this in a handful of seconds. The software will then display a "Module installed!" message.

![](<../../../../.gitbook/assets/51185193 (6) (9) (2).gif>)

Modules are not installed by default: you still have to click the module's "Install" button, and then possibly configure its settings via the "Installed modules" tab.

Once the configuration is complete, be sure to test the module immediately to confirm that it works as planned.

#### Installing using an FTP client <a href="#modulesselection-installingusinganftpclient" id="modulesselection-installingusinganftpclient"></a>

You can also choose to install a module by yourself, using an FTP client.

To install a new module manually:

1. Unzip (decompress) the module archive file (`.zip` or `tar.gz`). This should result in a new folder.
2. Using your FTP client, connect to the PrestaShop web server, and place the unpacked module folder in your installation's `/modules` folder.\
   Pay attention NOT to upload that folder in another module's folder (which can happen when drag-and-dropping items). **Upload both the folder and the files it contains, not just the files.**
3. Go to your back office, in the "Selection" tab.
4. Locate the new module in the modules list. You might have to scroll down; you can also use the list's search engine, which should give you a dynamically updated list of matching module names.
5. In the row for the new module, click the "Install" button.
6. Your module is now installed and should be activated too. If necessary, click on the module's "Configure" link. Also, pay attention to any warning message that might be displayed on your screen.

Once the configuration is complete, be sure to test the module immediately to confirm that it works as planned.

Modules can come from many sources, and not all of them are reliable. This is why PrestaShop software sometimes displays a warning window for "Untrusted" modules – that is, modules that have not been verified by PrestaShop. This screen window lets you choose whether to proceed with the installation with no further notification or to stop the installation process.
