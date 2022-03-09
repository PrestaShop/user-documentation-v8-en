# Database Backup

A backup is the action of saving the content of your database into files that you store in a safe place. The point is that you can revert to them in case your database fails on you.

You must perform regular backups of your shop, so that in case of a crash, you can reboot your shop quickly and in the best conditions. The database contains most of the information in your shop, many of which are indispensable for PrestaShop to work correctly – including your products, categories, and other data you added since the installation, but not your images for instance (these are stored, along with your theme files, on your server).

The more often you perform a backup, the safer you are. Once a week is a minimal frequency.

To create database backups of your shop, you have several solutions. You can use tools such as phpMyAdmin (reserved for advanced users), or use the one integrated into PrestaShop: the "DB backup" page.

The page starts with two big notices. You should read both completely in order to have a better idea of what the page does:

* The "Disclaimer" section gives you a series of reminders about backups, which you should read every time you make a backup. The section ends with the "I have read the disclaimer. Please create a new backup" button, which you have to click in order to create a backup. Once created, the backup appears in a new "Download section" at the top of the page (click the button in order to download the backup file to your computer), and in the list below the notices.
* The "How to restore" section gives you tips on how to get your data back into PrestaShop in case of failure. You should commit this to memory, or at least save this information somewhere in case a database crash makes it impossible for you to access the PrestaShop administration – and thus the DB backup page – again. Just in case, you will find it below as well.\
  \


How to restore a database backup in 10 easy steps

1. Set "Enable Shop" to "No" in the "Maintenance" page under the "Preferences" menu.
2. Download the backup from the list below or from your FTP server (in the folder "admin/backups").
3. Check the backup integrity: Look for errors, incomplete file, etc... Be sure to verify all of your data.
4. Please ask your hosting provider for "phpMyAdmin" access to your database.
5. Connect to "phpMyAdmin" and select your current database.
6. Unless you enabled the "Drop existing tables" option, you must delete all tables from your current database.
7. At the top of the screen, please select the "Import" tab
8. Click on the "Browse" button and select the backup file from your hard drive.
9. Check the maximum filesize allowed (e.g. Max: 16MB)
10. Click on the "Go" button and please wait patiently for the import process to conclude. This may take several minutes.

The table below the notices lists all the backups that have already been made, indicating the date of creation, age, file name, and size.\
At the right of each row are the available actions:

* **View**. Enables you to download this backup.
* **Delete**. Enables you to delete this backup. Be careful, there is no turning back.

![](<../../../../.gitbook/assets/23789873 (3) (4).png>)

After each backup process, you should download the generated backup file by clicking on its "View" icon, or simply by using the link in the notification box at the top. Put your backup file in a safe place, for you might need it at any given time. Furthermore, you can find these backups directly on your server, in the `/backup` folder, under your custom-named `/admin` folder.

Your database is saved using the standard SQL format and its `.sql` file extension, and compressed using the BZip2 algorithm (simply put, a variant of the popular Zip format. Read more: [http://en.wikipedia.org/wiki/Bzip2](http://en.wikipedia.org/wiki/Bzip2)) and its `.bz2` file extension. That gives a file archive with the `.sql.bz2` file extension

## Backup Options <a href="#databasebackup-backupoptions" id="databasebackup-backupoptions"></a>

At the bottom of the screen, two options are available:

*
  * **Ignore statistics tables**. PrestaShop stores your site's statistics in a handful of database tables, and these can grow big quite quickly. While it can be sound to keep your stats in a safe place, they also make for huge files to download, while you are probably more interested in a backup of your products, categories, customers, orders, etc.\
    By default, PrestaShop backups all tables, but if you are short on disk space on your web server, change this option to "Yes".
  * **Drop existing tables during import**. When importing a backup file, the system can either overwrite the existing live tables with the content of the ones that were backed up, or delete all existing in order to replace them with the content of the backup. The first case can result in doubles, which is why this option is enabled by default.\
    \
    ![](<../../../../.gitbook/assets/45580384 (4) (4) (1).png>)
