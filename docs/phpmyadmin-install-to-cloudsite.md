
# How to install phpMyAdmin

> GearHost does not provide a central phpMyAdmin log in area for customers. This is because phpMyAdmin is a 3rd party software utility that must be maintained and patched from time to time due to security releases. If you chose to install this software please make sure you do this yourself or risk having your phpMyAdmin software and or databases compromised. The software is also limited by some functionality that is provided by using MySQL Tools which we do fully support and encourage the use of. [Learn how to connect to your MySQL database using MySQL Tools](https://www.gearhost.com/documentation/connecting-to-mysql-database). As such if the below becomes complicated please revert to the link above to use our preferred method of connecting to MySQL.

### Installation
1. [Download the latest version of phpMyAdmin](https://www.phpmyadmin.net/downloads/)
2. **Extract the files** to your local computer
3. **Download** and **save** the following file: [config.inc.php](https://raw.githubusercontent.com/GearHost/docs/master/Images/files/config.inc.php)
4. **Open** `config.inc.php` and **update** the string "PLEASEUPDATEME" on **line 17** to any random letters & numbers.
5. This would be for cookie encryption. It can be something such as `123651b1561d891651` then **save** the file.
5. **Delete** the `setup directory` and `config.sample.inc.php` file.
6. You now have a working phpMyAdmin software folder
7. **Upload folder** to a **CloudSite** that you wish to host it on
8. **Use** a sub-folder called */phpmyadmin* for example.
7. You can now log in with your database user name and password as well as select which MySQL server you wish to connect to from the drop down list.