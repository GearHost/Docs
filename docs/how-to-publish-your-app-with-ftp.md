# Getting Started with FTP
Publishing your app using your favorite FTP client couldn't be easier with GearHost. As with all FTP clients you will need the hostname, username and password. If you don't have any FTP client installed, please be sure to check out our guide on installing [FileZilla here.](https://www.gearhost.com/documentation/installing-filezilla) 

### FTP credentials
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)

2. Click on your **CloudSite**

3. Select the **Publish** tab

   ​	If using FileZilla download the import profile. If not click the "eye" icon to view your FTP password. 	 	FTP hostname is: publish.gearhost.cloud

### Can I set my own password?
You cannot change the default FTP user acount password. You can reset passwords for created FTP users.

### Can I create another FTP user?
1. Click on **Add Publish User**
2. Fill out Username and Password
3. Click on **Create User**

You will now be able to use this newly created user to connect via FTP.

### Where do I upload my files?
The webroot directory for your CloudSite is **/webroot/**

### Import publishing file(s) in FileZilla
We provide a XML file that you can import to FileZilla. This file saves your FTP connection to the Site Manager which makes it easier to connect. On the same **Publish** menu, click on the FileZilla icon to download the XML file.

1. **Launch FileZilla**
2. Under the **File** menu select **Import...**
3. Browse for the **.xml file** you just downloaded
4. Select **OK** on the Import Settings dialog box
5. Select **OK** on the Import Successful confirmation box
6. Under the **File** menu select **Site Manager**
7. Under **My Sites** select your CloudSite and click **Connect**

