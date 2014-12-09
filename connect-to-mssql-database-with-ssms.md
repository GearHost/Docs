Connect To Microssoft SQL Server Management Studio 2014 (SSMS)
====

First you will need SQL Server Management Studio, You can download Sql Server Management Studio

[SSMS 2012](http://www.microsoft.com/betaexperience/pd/SQL2012EvalCTA/enus/default.aspx)

[SSMS 2014](http://msdn.microsoft.com/en-us/evalcenter/dn434042.aspx)

There are some features of you MSSQL database that you can manage through Microsoft SQL Management Studio. This article explains how to connect to your CloudSites database using that application. You will need the details of your database in order to do this. If you do not know your Database Details, you can find out what they are by [logging into your customer portal][login]. Clicking on the databases menu option, and click the name of the database you need details for.
	
![menu databases][menu-databases]

1. Open Microsoft SQL Management Studio. Choose Database Engine as the Server type.

2. The Server name will be mssql2.cloudsites.gearhost.com

3. Authentication will be SQL Server Authentication.

4. The Login will be the name of your database and the Password will be the password that is provided for you in the database details section in the control panel, under the database management module. The login dialog box in Microsoft SQL Management Studio should look something like this (with your password in the password field):
   
	![SSMS](https://support.gearhost.com/attachments/token/lndmqjpk4tkcng6/?name=SQLMS.PNG)

5. If the information has been entered correctly you will be able to connect successfully to your database.


[menu-databases]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/login.png
