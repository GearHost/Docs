# Connect to a MSSQL Database
This article covers 3 steps needed to connect to your hosted Microsoft SQL Server database. To connect to a MySQL database [click here](https://www.gearhost.com/documentation/connect-to-a-mysql-database).

### Step 1: Install SQL Server Management Studio (SSMS)
1. Download and install [the last version of SQL Server Management Studio](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms)

### Step2: Find your Database Information
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Click the Databases menu
3. Locate the Database you want to connect to and click it to open the database details
4. Note the server name for example `den1.mssql1.gear.host`, username and password (click on the "eye" icon to reveal your password)

> Your username is the same name as your database name. This is your primary database user which cannot be deleted and is the only user that is allowed access to your database using SSMS. Additional users do not have this access.

### Step 3: Connect to your database using SSMS
1. Launch Microsoft SQL Server Management Studio
2. The Server type should be *Database Engine*
3. Enter the server name (see above)
4. Authentication is *SQL Server Authentication*
5. Enter your database username (see above)
6. Enter your database password (see above)
7. Click Connect

If you have any questions let us know and [open a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket).