#Connecting to a SQL database using SQL Server Management Studio (SSMS)

This article covers 3 steps needed to connect to your hosted MSSQL database.

###Install SQL Server Management Studio 2016 (SSMS)
1. Download and install [SQL Server Management Studio 2016](https://www.microsoft.com/en-us/download/details.aspx?id=42299)

> GearHost uses SQL Server 2016 and older versions of SQL Server Management Studio will not work correctly. Please ensure you are using SSMS 2016.

###Locate your database username, password and server name
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Click the Databases menu
3. Locate the Database you want to connect to and click it to open the database details
4. Your username is the same name as your database. This is your primary database user that we create for you by default and the only user that can connect to your database using SSMS.
5. Toggle the show/hide password by clicking on the "eye" icon to the right of the username to see the password.
6. You will need the server name located at the bottom. The format is `mssqlx.gear.host`.

> Note that only your primary username can connect to the SQL server database using SSMS. While additional users have access to your database in your application they do not have access via SSMS.

###Connect to your database using SSMS
1. Launch Microsoft SQL Server Management Studio 2016
2. The Server type should be *Database Engine*
3. Server name should be `mssqlx.gear.host` (see above)
4. Authentication is *SQL Server Authentication*
5. Enter your database username (see above)
6. Enter your database password (see above)
7. Click Connect

If you have any questions let us know and [open a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket).