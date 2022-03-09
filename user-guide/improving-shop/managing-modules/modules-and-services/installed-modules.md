# Installed modules

On this page, you can install, uninstall, configure and update each of your modules. This chapter simply explains how you can manage your modules from the "Installed modules" tab.

![](<../../../../.gitbook/assets/51185201 (5) (3) (3).png>)

## The modules list <a href="#installedmodules-themoduleslist" id="installedmodules-themoduleslist"></a>

This list enables you to quickly find the module you want to configure or edit the settings of.

It is divided into 3 sections:

* **Installed modules**. These are all the modules you’ve added to your shop, either by buying it from PrestaShop Addons, or by uploading it directly.
* **Built-in modules**. These modules from PrestaShop are preinstalled when you set-up your shop. They cover the basics of e-commerce and comes for free.
* **Theme modules**. Each theme you install will come with its own set of modules. You’ll find here all the modules related to your active theme.

If you want to quickly find a module, you can search for a specific module, or filter down modules until you find the one you are looking for.

![](<../../../../.gitbook/assets/51185200 (5) (2) (3).png>)

* **Search field**. Search for a module with its name, author or with keywords.
* **Sort selectors**. The list automatically reloads when you make a selection, and displays modules according to all the current settings.
  * **Categories**. On the left is a list of all the module categories, with the number of modules for each in brackets. Click on a category in order to display the modules for this category.
  * **Show all modules.** Allows you to choose between enabled and disabled modules. Enabled modules are the only ones that can be configured, hence the importance of this selector.
  * **Installed & Not Installed**. Most of the time, you will want to perform an action on an installed module or install a new one. This filter is the most commonly used.
  * **Last access.** If you often use the same modules, this option will make it easier to find the latest modules you have been working on.
  * **Name**. Sorts modules by alphabetical order, from A to Z.

Modules can have one of 4 statuses:

* Non-installed.
* Installed but disabled
* Installed and enabled.
* Installed and enabled, but with warnings.\
  \


Difference between disabling and uninstalling

When you do not have a use for a module anymore, you can either disable or uninstall it. The results of both actions are seemingly the same: the module is not available anymore, its options do not appear in your back office and any element it added to your front-end have disappeared.

The difference is that disabling a module keeps its configuration safe for later re-enabling while uninstalling it removes all of its configuration and database data. All the module's files will be deleted.

Therefore, you should only uninstall a module if you do not care about its data or if you are certain that you would not need it. It is like deleting it for good.

## Performing Actions on Modules <a href="#installedmodules-performingactionsonmodules" id="installedmodules-performingactionsonmodules"></a>

Here are the available actions, depending on the module's status:

* Uninstalled modules:
  * **Install**. This will trigger the installation of the module on your installation of PrestaShop. The module will be automatically enabled.\
    \

* Installed modules:
  * **Upgrade**. Your PrestaShop installation regularly checks with the Addons server if there is any update for your modules. If so, the action button becomes "Upgrade" for the affected modules. Simply click it, and PrestaShop will take care of downloading and updating the module.
  * **Enable**. For modules which have been formerly disabled. Once enabled again, it might add new options to your back office.
    * **Enable on mobile**. This will enable the front office view of the module only for mobile devices (smartphones, etc.).
  * **Configure**. Some modules have a configuration page. In that case, they offer a "Configure" link to access a new interface where the user will be able to adjust all its settings.
  * **Disable**. When installed, a module is enabled by default. You can disable it, which will remove its options from your back office but will keep its settings for a later re-enabling.
    * **Disable on mobile**. This will disable the front office view of the module only for mobile devices (smartphones, etc.).
  * **Reset**. This will restore the module's settings to their defaults.
  * **Uninstall**. This will disable the module. To also delete all its files and data, you should select the option "Delete module folder after uninstall."

These actions can be performed either individually on each module, or in mass thanks to the "Bulk actions" menu on the right.

### Uninstalling a module <a href="#installedmodules-uninstallingamodule" id="installedmodules-uninstallingamodule"></a>

**Do not ever delete a module by directly trashing its folder using your FTP client!** You must let PrestaShop take charge of it.

When you need to temporarily stop using a module, but still wish to keep its configuration, you can simply disable it: just click on the "Disable" link. The actions will turn into "Enable" and "Delete", but the "Uninstall" button can still be seen.

If you do not care about the module's configuration, click on the "Uninstall" button: your module's folder will still be in the `/modules` folder, but the module will not have any impact on your shop anymore.\
If you wish to entirely remove the module from your server, click the "Delete" link: PrestaShop will get rid of its folder and all its files.

Make sure that the disabling or removal of the module does not break the theme.
