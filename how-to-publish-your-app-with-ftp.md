How to publish your app with FTP
==================

Below we'll walk through setting up deployment credentials and using those in an FTP client to publish your application to your account. 

>Create your deployment credentials 

 1. After logging into your control panel click on CloudSites and choose the site you want to publish to. 
 
 2. Click on the button Set Deployment Credentials.
 
 3. Type in a user name and password you would like to use and click change password. *It's important to note that your deployment credentials are used for all your CloudSites. When you set or change them on one CloudSite it will change the password for your other CloudSites. Each CloudSite will have a different user name though.* 
 
 4. Now that you have your credentials you can enter them into an FTP client like [FileZilla](https://filezilla-project.org/download.php?type=client). You can find the server address on the same page in the control panel as where you configured your deployment credentials, ftp.gear.host Your user name is also there. *Note that the user name includes your CloudSite name. In the example below "example1" is the name of my CloudSite, "ftpuser1" is the user I created for deployment. Each CloudSite will use the deployment credentials CloudSiteName\UserName and the same password. This will make it easier for you when you add your next CloudSite. All you'll need to remember is the CloudSite name and the user name.*
 
 ![quick glance deployment information][quick-glance]


 
> Enter your credentials in FileZilla
 

 1. Open FileZilla and in the quick connect bar enter the server, user name, and password. Remember you can find the information on the Overview page of your CloudSite in your control panel.
 
 ![enter image description here](http://i.imgur.com/jpBnhEq.png)
 
 2. Click Quickconnect and you will be connected to the FTP server. 
 
 3. Now you will be able to upload your application or website content. Your content should be uploaded to /site/wwwroot.

[quick-glance]: https://raw.githubusercontent.com/GearHost/docs/master/Images/quick-glance.png
 
