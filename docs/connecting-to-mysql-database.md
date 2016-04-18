#How to connect to a MySql Database using SQL MySQL Workbench

This article covers 3 steps needed to connect to your MySQL database hosted with GearHost. The steps are:

1. [Download and Install MySQL WorkBench](https://www.gearhost.com/documentation/connecting-to-mysql-database#user-content-download-and-install-mysql-workbench)
2. [Gather your SQL Server database credentials](https://www.gearhost.com/documentation/connecting-to-mysql-database#user-content-gather-your-mysql-server-database-credentials)
3. [Connect to your SQL Server Database using SSMS](https://www.gearhost.com/documentation/connecting-to-mysql-database#user-content-log-in-to-mysql-workbench-with-your-credentials)

##Download and Install MySQL WorkBench
1. Download and install [MySQL WorkBench](https://dev.mysql.com/downloads/workbench/)

	> Note that GearHost uses MySQL server 6 and older versions of MySQL workbench may not connect due to new password complexity and encryption methods

##Gather your MySQL Server database credentials

1. Log in to your [GearHost portal.](https://my.gearhost.com)
1. Click on the **Databases** menu.
	
	

1. Locate the database you want to connect to and select it to go to Database Details

	

1. Locate the username that is the same name as your database. This is your primary database user that we create for you by default.

1. Toggle the show/hide password "eye" icon to the right of the user name to show the password.



1. At the bottom of the page take note of the SQL Server Name which you will use. It's format is *mysql#.gear.host*.



##Log in to MySQL Workbench with your credentials

1. Launch MySQL Workbench
1. Select database -> connect to database

	

1. Enter your Database server and username
 
	- Hostname should be *mysql#.gear.host* (refer to your steps above to determine the correct SQL Server name)
	- Log in is your primary database user name, the same name as your database name

	

1. Store your password in the vault then select ok
	
	> Your password is the password as reviled above using the show/hide password toggle icon above.



4. Confirm by selecting OK
5. You are now connected!

----------
**Tip:** Still having issues? Please open a support ticket and we'lll be glad to help you out!