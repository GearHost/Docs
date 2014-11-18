Free Database Suspension
==================

##Introduction
If you are receiving an error indicating your website or application cannot login to your database and you have a free database, the database may be suspended. Free databases have limits and if you go over those limits the database is suspended. 


##Free Database Limits
**MySQL**

- 5MB storage limit. This is the amount of disk space the database can consume
- Limited Connections. The number of active connections a database can have.

**MSSQL**

- 10MB storage limit. This is the amount of disk space the database can consume
- Limited Connections. The number of active connections a database can have.

***
##Errors
Examples of errors you may see if your database is suspended. 

**MSSQL**

*PDOException: SQLSTATE[42000]: [Microsoft][SQL Server Native Client 11.0][SQL Server]Login failed for user 'example'. Reason: The account is disabled. in db_table_exists() (line 2761 of C:\inetpub\temp\DWASFiles\Sites\example\VirtualDirectory0\site\wwwroot\includes\database\database.inc).*

*Login failed for user 'example'. Reason: The account is disabled. (Microsoft SQL Server, Error: 18470)*

![](http://i.imgur.com/SyLlw0z.png)

**MySQL**

*Could not connect: Access denied for user 'example'@'CSSITESSHARED10' (using password: YES)*

![](http://i.imgur.com/Wc6ei0c.png)

**Wordpress example**

*Error establishing a database connection*

![](http://i.imgur.com/vaOF5Hb.png)

Or you may see a 500 error depending on if you allow detailed error messages or not. 

*The website cannot display the page
HTTP 500 
Most likely causes:
The website is under maintenance.
The website has a programming error.*

![](http://i.imgur.com/Yyi0xEg.png)

##Control Panel
In the control panel when you click on databases you will see the following. 



##How to upgrade
Upgrading is simple, just follow the steps below. 

1. Login to your control panel at [https://my.gearhost.com](https://my.gearhost.com).
2. Click on Databases from the left hand side. 
3. Click on the upgrade link in the plan column next to the database you wish to upgrade. 

    ![](http://i.imgur.com/vFjPbvC.png)

4. Click yes on the prompt to upgrade the database. You will need a credit card on file to complete this action. 


####Still need help?
If you have any other questions that aren't covered in this documentation, feel free to e-mail <help@gearhost.com>.