# Publishing Your Site via WebMatrix 3

This article covers three steps needed to publish your website to Octane with WebMatrix 3. The steps are:

1. [Download Your Publishing File](https://www.gearhost.com/documentation/publish-via-webmatrix-3# user-content-download-your-publishing-file)
2. [Import Publishing File Into WebMatrix 3](https://www.gearhost.com/documentation/publish-via-webmatrix-3# user-content-import-publish-file-into-webmatrix-3)
3. [Publish Your Site](https://www.gearhost.com/documentation/publish-via-webmatrix-3# user-content-publish-your-site)
4. [Set up your Database](https://www.gearhost.com/documentation/publish-via-webmatrix-3# user-content-set-up-your-database)


#  Download your publishing file
1. [Log in][login-link]  to your account
2. Click on the CloudSite you wish to get the publishing file for
3. Click the Publish tab inside CloudSite details
4. Download publishing file by selecting the Visual Studio button under the Application Publishing Files title

> If you reset your publishing password you will need to download your publishing file again and re-import it.

#  Import Publish File into WebMatrix 3
1. Click on the Remote file menu
2. Click publish
3. Import publish profile
4. Set database (only if needed)
	1. Locate your server
	2. Enter the credentials
	3. Password and username for the database are located under the database user section
5. Validate connection

	

 >You can skip the test publish compatibility if you wish, the server is compatible with all static, Visual Basic, and .NET code.

#  Publish Your Site

When publishing your site from WebMatrix 3 you will receive a dialog showing you the changed files in your local project vs what is on the server.  There will be an option to delete all files on the server that are not in your local development project.  

 

 - Visit test URL provided for your site
 
 >This test URL should be in the format of `http://{cloudsitename}.gear.host` where you replace `{cloudsitename}` with the name of your CloudSite

#  Set Up Your Database

>There is currently a known issue with certain characters that are auto generated when you setup your database. If you are unable to connect to your database when using a publishing file go into your database in your account and change the password. The know characters are `*()/"'`  so do avoid them when creating a new password.

1. Create a new database by going to your database menu
2. Set a Database name
3. Select the database you need, either MySQL or MSSQL
4. Select create empty database
5. Set your password on the database to avoid the known issue of certain characters causing an issue during publishing

If you need to set up a connection to your database for management please follow the instructions in the articles below based on your database type.
   
- [MSSQL](https://www.gearhost.com/documentation/connect-to-a-mssql-database)
- [MySQL](https://www.gearhost.com/documentation/connecting-to-mysql-database)


[Login-Link]:https://my.gearhost.com/account/login

[menu-cloudsites]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-cloudsites.png
[select-cloudsite]: https://raw.githubusercontent.com/GearHost/docs/master/Images/select-cloudsite.png
[download-publishing-file]: https://raw.githubusercontent.com/GearHost/docs/master/Images/publishfile.png

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

>**Tip:** You can publish your application using different methods. Such options include; [Visual Studio](https://www.gearhost.com/documentation/how-to-publish-your-app-from-visual-studio), [Git](https://www.gearhost.com/documentation/github-deploy-your-application), and [FTP](https://www.gearhost.com/documentation/how-to-publish-your-app-with-ftp)! If you're still having an issue, please don't hesitate to [open a support ticket.](https://www.gearhost.com/documentation/how-to-open-a-support-ticket)