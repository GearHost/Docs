#Publishing Your Site via WebMatrix 3

This article covers three steps needed to publish your website to Octane with WebMatrix 3. The steps are:

1. [Download Your Publishing File](https://www.gearhost.com/documentation/publish-via-webmatrix-3#user-content-download-your-publishing-file)
2. [Import Publishing File Into WebMatrix 3](https://www.gearhost.com/documentation/publish-via-webmatrix-3#user-content-import-publish-file-into-webmatrix-3)
3. [Publish Your Site](https://www.gearhost.com/documentation/publish-via-webmatrix-3#user-content-publish-your-site)

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

 - Validate connection

	![validate connection][webmatrix-validate-connection]

 >You can skip the test publish compatibility if you wish, the server is compatible with all static, Visual Basic, and .NET code.

###Publish Your Site

When publishing your site from WebMatrix 3 you will receive a dialog showing you the changed files in your local project vs what is on the server.  There will be an option to delete all files on the server that are not in your local development project.  


 
   ![publish preview][webmatrix-publish-preview]

 - Visit test URL provided for your site
 
 >This test URL should be in the format of **http://cloudsitename.geat.host** where you replace cloudsitename with the name of your CloudSIte

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