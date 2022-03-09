---
description: PrestaShop also has an installer for command-line installations.
---

# Installing PrestaShop using the command-line script

## What is it? <a href="#installingprestashopusingthecommand-linescript-whatitis" id="installingprestashopusingthecommand-linescript-whatitis"></a>

This special installer makes it possible to install PrestaShop without the need to use a web browser: simply put the content of the zip archive on your web server, and you can install PrestaShop through your command-line interface (CLI). Any CLI software can be used as long as you can use it to interact with the server's commands: Bash, Windows PowerShell, OS X Terminal, PuTTY, etc.

The point of having a CLI installer in addition to the regular in-browser installer is to give this option to cater for some advanced users, who often prefer command-line interfaces as they tend to provide a more concise and powerful means to control a program or operating system.

## How to use it? <a href="#installingprestashopusingthecommand-linescript-howtouseit" id="installingprestashopusingthecommand-linescript-howtouseit"></a>

The CLI installer is easy to use: from your terminal, go to the `/install` (or `/install-dev`) folder (meaning you have previously unzipped the pestashop.zip file), and start the script with this command:

```
$ php index_cli.php
```

This will display the various available options.

![](<../.gitbook/assets/54264260 (1) (5).png>)

All the options from the regular in-browser installer are available, with their default value listed. Almost all default values can be left as is, because you can edit them all from the PrestaShop back office once the installation is done. Note that the e-mail and password are the ones used to create the administrator's back office account...

To start the installation, you only need to provide one argument. In reality, you need to provide more:

* **domain**. The location where you want your store to appear.
* **db\_server**. The database server address.
* **db\_name**. The name of the database you want to use.
* **db\_user**. The username for the database you want to use.
* **db\_password**. The password for the database username above.

For instance:

```
$ php index_cli.php --domain=example.com --db_server=sql.example.com --db_name=prestashop --db_user=root --db_password=123456789
```

![](<../.gitbook/assets/53641264 (6).png>)

If you also set the `--email` value to your own address, a recap e-mail will be sent to you once the installation is done.

## List of arguments <a href="#installingprestashopusingthecommand-linescript-listofarguments" id="installingprestashopusingthecommand-linescript-listofarguments"></a>

Here is the list of arguments for index\_cli.php as of version 1.6:

| Name             | Default setting                                 | Description                                           |
| ---------------- | ----------------------------------------------- | ----------------------------------------------------- |
| --step           | process                                         |                                                       |
| --language       | en                                              | language iso code                                     |
| --timezone       | localhost                                       |                                                       |
| --domain         | localhost                                       |                                                       |
| --db\_server     | localhost                                       |                                                       |
| --db\_user       | root                                            |                                                       |
| --db\_password   | (blank)                                         |                                                       |
| --db\_name       | prestashop                                      |                                                       |
| --db\_clear      | 1 (true)                                        | Drop existing tables                                  |
| --db\_create     | 0 (false)                                       | Create the database if it does not exist yet          |
| --prefix         | ps\_                                            |                                                       |
| --engine         | InnoDB                                          | InnoDB/MyISAM                                         |
| --name           | PrestaShop                                      | Name of the shop                                      |
| --activity       | 0                                               |                                                       |
| --country        | fr                                              |                                                       |
| --firstname      | John                                            |                                                       |
| --lastname       | Doe                                             |                                                       |
| --password       | 0123456789                                      |                                                       |
| --email          | [pub@prestashop.com](mailto:pub@prestashop.com) |                                                       |
| --license        | 0 (false)                                       | Show PrestaShop's license                             |
| --newsletter     | 1 (true)                                        | Subscribe administrator to PrestaShop's newsletter    |
| --send\_email    | 1 (true)                                        | Send an email to the administrator after installation |
| --all\_languages | 0 (false)                                       | Install all the existing languages on the shop        |
| <p>--ssl<br></p> | 0 (false)                                       | (From PS 1.7.4) Enable HTTPS on the shop              |
