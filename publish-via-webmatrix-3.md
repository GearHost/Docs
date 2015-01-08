#Publishing Your Site via WebMatrix 3

This article covers three steps needed to publish your website to Octane with WebMatrix 3. The steps are:

1. [Download Your Publishing File](https://www.gearhost.com/documentation/publish-via-webmatrix-3#user-content-download-your-publishing-file)
2. [Import Publishing File Into WebMatrix 3](https://www.gearhost.com/documentation/publish-via-webmatrix-3#user-content-import-publish-file-into-webmatrix-3)
3. [Publish Your Site](https://www.gearhost.com/documentation/publish-via-webmatrix-3#user-content-publish-your-site)
4. [Set up your Database](https://www.gearhost.com/documentation/publish-via-webmatrix-3#user-content-set-up-your-database)


###Download your publishing file

 - [Log in][login-link]  to your account

 - Select your CloudSite
 	
	![select cloudsite][select-cloudsite]

 - Download publishing pile

	![downloading publishing file][download-publishing-file]

> If you reset your publishing file you will need to redownload the publishing file and re-import it as the password will have changed.

###Import Publish File into WebMatrix 3

 - Click on the Remote file menu
 - Click publish

	![webmatrix 3 menu][menu-webmatrix]


 
 - Import publish profile
 
	![webmatrix import publish][webmatrix-import-publish-file]

 - Set database (only if needed)
	- Locate your server
	
	![menu-locateserver][menu-locateserver]
	- Enter the credentials
	
	![webmatrix-destination][webmatrix-destination]

	- Password and username for the database are located under the database user section

	![database-viewpass][database-viewpass]
 - Validate connection

	![validate connection][webmatrix-validate-connection]

 >You can skip the test publish compatibility if you wish, the server is compatible with all static, Visual Basic, and .NET code.

###Publish Your Site

When publishing your site from WebMatrix 3 you will receive a dialog showing you the changed files in your local project vs what is on the server.  There will be an option to delete all files on the server that are not in your local development project.  

 
   ![publish preview][webmatrix-publish-preview]

 - Visit test URL provided for your site
 
 >This test URL should be in the format of **http://cloudsitename.geat.host** where you replace cloudsitename with the name of your CloudSIte

###Set Up Your Database

>There is currently a known issue with certain characters that are auto generated when you setup your database. If you are unable to connect to your database when using a publishing file go into your database in your account and change the password. The know characters are * ( ) /  so do avoid them when creating a new password.

1. Create a new database by going to your database menu 


	![database-menu][database-menu]
2. Set a Database name


	![database-name][database-name]
3. Select the database you need, either MySQL or MSSQL

	![database-selectplan][database-selectplan]
3. Select create empty database

	![database-empty][database-empty]
4. Set your password on the database to avoid the known issue of certain characters causing an issue during publishing 
	 
	![database-password][database-password]


If you need to set up a connection to your database for management please follow the instructions in the articles below based on your database type.
   
- [MSSQL](https://www.gearhost.com/documentation/connecting-to-a-sql-database-using-sql-server-management-studio-2014)
- [MySQL](https://www.gearhost.com/documentation/connecting-to-mysql-database)


[Login-Link]:https://my.gearhost.com/Account/Login

[menu-cloudsites]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-cloudsites.png
[select-cloudsite]: https://raw.githubusercontent.com/GearHost/docs/master/Images/select-cloudsite.png
[download-publishing-file]: https://raw.githubusercontent.com/GearHost/docs/master/Images/download-publishing-file.png

[menu-webmatrix]: https://raw.githubusercontent.com/GearHost/docs/master/Images/webmatrix-3-file-menu.png
[webmatrix-import-publish-file]: https://raw.githubusercontent.com/GearHost/docs/master/Images/webmatrix-import-publish-file.png
[webmatrix-validate-connection]: https://raw.githubusercontent.com/GearHost/docs/master/Images/webmatrix-validate-connection.png
[webmatrix-publish-preview]: https://raw.githubusercontent.com/GearHost/docs/master/Images/webmatrix-publish-preview.png
[webmatrix-destination]: https://raw.githubusercontent.com/GearHost/docs/master/Images/webmatrix-destination.png
[menu-locateserver]: https://raw.githubusercontent.com/GearHost/docs/master/Images/mssql-db-server.png
[database-viewpass]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-showhidepassword.png

[database-menu]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[database-password]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-resetpassword.png
[database-name]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-namedb.png
[database-selectplan]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-selectplan.png
[database-empty]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-createempty.png