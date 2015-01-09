#How to connect to a MySql Database using SQL MySQL Workbench

This article covers 3 steps needed to connect to your MySQL database hosted with GearHost. The steps are:

1. [Download and Install MySQL WorkBench](https://www.gearhost.com/documentation/connect-to-sql-server#user-content-install-sql-server-management-studio-2014-ssms)
2. [Gather your SQL Server database credentials](https://www.gearhost.com/documentation/connect-to-sql-server#user-content-gather-your-sql-server-database-credentials)
3. [Connect to your SQL Server Database using SSMS](https://www.gearhost.com/documentation/connect-to-sql-server#user-content-connect-to-your-sql-server-database-using-ssms)

##Download and Install MySQL WorkBench
1. Download and install [MySQL WorkBench 6.2][mysql-workbench-link]

	> Note that GearHost uses MySQL server 6 and older versions of MySQL workbench may not connect due to new password complexity and encryption methods

##Gather your MySQL Server database credentials

1. [Log in to your GearHost Account][Login-Link]
1. Click on the Databases menu
	
	![dbtab][db-tab]

1. Locate the database you want to connect to and select it to go to Database Details

	![selectdb][select-db]	

1. Locate the username that is the same name as your database. This is your primary database user that we create for you by default.

	![showhide][show-hide]

1. Toggle the show/hide password "eye" icon to the right of the username to show the password.
1. At the bottom of the page take note of the SQL Server Name which you will use. It's format is *mysql#.gear.host*.



##Log in to MySQL Workbench with your credentials

1. Launch MySQL Workbench
1. Select database -> connect to database

	![wbdb][workbench-db]

1. Enter your Database server and username
 
	- Hostname should be *mysql#.gear.host* (refer to your steps above to determine the correct SQL Server name)
	- Login is your primary database username, the same name as your database name

	![wb-creds][enter-creds]

1. Store your password in the vault then select ok
	
	> Your password is the password as reviled above using the show/hide password toggle icon above.

	![vault]

4. Confirm by selecting OK
5. You are now connected!



[mysql-workbench-link]: http://dev.mysql.com/downloads/workbench
[menu-databases]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[Login-Link]:https://my.gearhost.com/Account/Login
[db-tab]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[select-db]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-select-db.png
[show-hide]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-database-showhidepassword.png
[db-details]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-db-server.png
[mssql-db-login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-db-login.png


[restore]: https://www.gearhost.com/documentation/how-to-restore-a-database
[db-tab]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[select-db]: https://raw.githubusercontent.com/GearHost/docs/master/Images/select-db.png
[show-hide]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-showhidepassword.png
[db-details]: https://raw.githubusercontent.com/GearHost/docs/master/Images/db-server.png
[workbench-db]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-workbenchdatabase.png
[enter-creds]: https://raw.githubusercontent.com/GearHost/docs/master/Images/workbench-enter-creds.png
[vault]: https://raw.githubusercontent.com/GearHost/docs/master/Images/workbench-vault.png
