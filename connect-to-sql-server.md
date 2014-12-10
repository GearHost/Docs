Connecting to your SQL Server database using Microssoft SQL Server Management Studio 2014 (SSMS)
====

First you will need SQL Server Management Studio which is free. You can download Sql Server Management Studio using the following link from Microsoft:

[SQL Server Management Studio 2014](http://msdn.microsoft.com/en-us/evalcenter/dn434042.aspx)

Once you download and install SQL Server Management Studio you can connect using your database credentials. To get your database credentials please follow these steps:

1. Login


There are some features of you MSSQL database that you can manage through Microsoft SQL Management Studio. This article explains how to connect to your CloudSites database using that application. You will need the details of your database in order to do this. If you do not know your Database Details, you can find out what they are by [logging into your customer portal][login-link]. Clicking on the databases menu option, and click the name of the database you need details for.
	
1. Get your credentials
	
	a. Select your database tab
	
	b. Select the database

    ![selectdb][select-db]

	c. Select Show/Hide Password to seee your password
	
	![showhide][show-hide]
	
	d. Note your username and password under the database users, and database server under the database details
	
	![dbdetails][db-details]

2. Open Microsoft SQL Management Studio. Choose Database Engine as the Server type.

3. The Server name will be sql01.gear.host

4. Authentication will be SQL Server Authentication.

5. The Login will be the name of your database and the Password will be the password that is provided for you in the database details section in the control panel, under the database management module. The login dialog box in Microsoft SQL Management Studio should look something like this (with your password in the password field):
   
	![SSMS][mssql-db-login]

6. If the information has been entered correctly you will be able to connect successfully to your database.


[menu-databases]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[Login-Link]:https://my.gearhost.com/Account/Login
[db-tab]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[select-db]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-select-db.png
[show-hide]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-database-showhidepassword.png
[db-details]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-db-server.png
[mssql-db-login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-db-login.png
