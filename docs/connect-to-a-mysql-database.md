# Connect To a MySQL Database
This article covers 3 steps needed to connect to your hosted MySQL database.

### Install MySQL WorkBench
1. Download and install [MySQL WorkBench](https://dev.mysql.com/downloads/workbench/)

> GearHost uses MySQL server version 5.X, older versions of MySQL Workbench may not connect. Please ensure you are using MySQL Workbench 6.X

### Locate your database username, password and server name
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Click the Databases menu
3. Locate the Database you want to connect to and click it to open the database details
4. Your username is the same name as your database. This is your primary database user that we create for you by default.
5. Toggle the show/hide password by clicking on the "eye" icon to the right of the username to see the password.
6. You will need the server name located under **Database Server**. The format is `den1.mysqlX.gear.host`

Note: *You will need to change the X to match the number displayed in the database details page.*

### Connect to your database using MySQL Workbench
1. Launch MySQL Workbench
2. From the menu select Database > Connect to Database
3. Enter the hostname with the database server name (see above)
4. Leave the default port of 3306
5. Enter your database username (see above)
6. Click Ok
7. When asked for your password enter it (see above)
8. Click on the tile to connect to your database

If you have any questions let us know and [open a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket).