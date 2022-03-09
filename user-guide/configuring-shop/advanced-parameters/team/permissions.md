# Permissions

Permissions are the central part of PrestaShop's profiles. They enable you to see very precisely what an employee account can and cannot do on your shop.

The "Permissions" administration page is built using tabs:

* On the left of the screen, as many tabs as there are available profiles.
* On the remaining right of the screen, PrestaShop displays the selected profile's permissions. This tab contains two tables side by side.

When you click any profile (except SuperAdmin), the two tables appear to give you access to their criteria:

* On the left, menu-related permissions: you can decide what the profile can do with menus. In effect, you could prevent a profile from editing the content of a page, or even hide the menu entirely.
* On the right, module-related permissions: while you might allow some profiles to see the available modules, you might prefer that only the most trustworthy employees should be able to configure some key modules.&#x20;

![](<../../../../.gitbook/assets/43417612 (2) (1) (3).png>)

For each of the menu criteria, you have 5 options:

* **View**. Employee can view information.
* **Add**. Employee can add new information.
* **Edit**. Employee can change information.
* **Delete**. Employee can delete information.
* **All**. Enable all the above options for the current row.

Meanwhile, the module criteria have 3 options:

* **View**. Employee can view the module's configuration.
* **Configure**. Employee can configure the module.
* **Uninstall**. Employee can uninstall the module.

The SuperAdmin permissions cannot be changed: the profile simply has all the rights for every criterion.

## Setting permissions for a new profile <a href="#permissions-settingpermissionsforanewprofile" id="permissions-settingpermissionsforanewprofile"></a>

For this example we will create a new profile, "Order Preparer". First create the profile in the "Profiles" page, by filling the "Name" field. As soon as it is saved, it appears in the list of profiles.

Then you need to assign permissions to this new profile. Go to the "Permissions" page, and click on the tab for the new profile: the list of criteria appears. By default, a new profile has access to none of the back office pages.

There are two ways to fill the criteria, depending on the limits or freedom you want the profile to have:

* Click the permission checkboxes one by one until it has enough access rights to get the job done.
* Have all the checkboxes checked, then remove permissions one by one until it has only the ones necessary.

You have two ways to have checkboxes checked in batches:

* Per column: at the top of each column, a checkbox makes it possible to have all of the column's checkboxes checked at once. Unchecking it unchecks all the currently checked boxes.
* Per row: if you click on the "All" checkbox for a given row, all the checkboxes this row will be checked. Unchecking it unchecks all the currently checked boxes.

You can then uncheck selected rows rather than spending time checking each needed rows one by one.

To avoid mistakes during the configuration of your permissions, PrestaShop automatically saves your settings every time you make a change. This means you do not have to click any "Save" button. Once you have assigned the profile its rights, you can return to the "Employees" administration page and start assigning that new profile to the employees who need it.
