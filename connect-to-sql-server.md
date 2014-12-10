Connecting to a SQL Database using SQL Server Management Studio
====

First you will need to install SQL Server Management Studio 2014 which is free. You can download Sql Server Management Studio using the following link from Microsoft:

[SQL Server Management Studio 2014](http://msdn.microsoft.com/en-us/evalcenter/dn434042.aspx)

> Note that GearHost uses SQL 2014 and older versions of SQL Server Management Studio are not supported.

Once you download and install SQL Server Management Studio you can connect using your database credentials. To get your database credentials please follow these steps:

1. [Log in to GearHost](https://my.gearhost.com/account/login)
2. Click on the Databases menu
3. Locate the database you want to connect to and select it to go to Database Details
4. Locate the username that is the same name as your database. This is your primary database user that we create for you by default.
5. Toggle the show/hide password "eye" icon to the right of the username to show the password.
6. At the bottom of the page take note of the SQL Server Name which you will use. It's format is *sqlx.gear.host*.

> Note that ONLY your primary username can connect to the SQL Server database using Microsoft SQL Server Management Studio. While additional users have access to your database in your code they do not have access via SSMS.

1. Launch Microsoft SQL Server Management Studio 2014
2. The Server type should be *Database Engine*
3. Server name should be *sqlx.gear.host* (refer to your steps above to the correct SQL Server)
4. Authentication is *SQL Server Authentication*
5. Login is your primary database username, the same name as your database name
6. Your password is the password as revield above using the show/hide password toggle icon.

For example your connection should look like this:

![SSMS][mssql-db-login]


[menu-databases]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[Login-Link]:https://my.gearhost.com/Account/Login
[db-tab]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[select-db]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-select-db.png
[show-hide]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-database-showhidepassword.png
[db-details]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-db-server.png
[mssql-db-login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-db-login.png
