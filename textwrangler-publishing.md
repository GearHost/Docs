How to publish your app with TextWrangler
==================

Below we'll walk through setting up deployment credentials and using them to publish your site through TextWrangler

>Create your deployment credentials 

 1. After logging into your control panel click on CloudSites and choose the site you want to publish to. 
 
 2. Click on the button Set Deployment Credentials.
 
 3. Type in a user name and password you would like to use and click change password. *It's important to note that your deployment credentials are used for all your CloudSites. When you set or change them on one CloudSite it will change the password for your other CloudSites. Each CloudSite will have a different user name though.* 
 
 4. Now that you have your credentials you can enter them into an FTP client like [FileZilla](https://filezilla-project.org/download.php?type=client). You can find the server address on the same page in the control panel as where you configured your deployment credentials, ftp.gear.host. Your user name is also there. *Note that the user name includes your CloudSite name. In the example below "example1" is the name of my CloudSite, "ftpuser1" is the user I created for deployment. Each CloudSite will ...(line truncated)...
 
 ![enter image description here][quick-glance]


 
> In TextWrangler, once you have finished building your pages, you can upload them easily to your CloudSites using the built in FTP function. These instructions can work for other content editors but may be slightly different.
 

 1. With the file open you would like to upload to your server, slect *File* from the Menu bar the select *Save to ftp/sftp server*
 ![Imgur](http://i.imgur.com/LBlY7ts.png)
 2. At the next pop-up screen, name your file then click *connect*. You will be asked to enter the server name and credentials which we have created already in our CloudSites control panel.
 ![Imgur](http://i.imgur.com/fSkCBZp.png)
 3.Once connected, save your file to the correct location then click *save*. You files are now saved on CloudSites servers!


[quick-glance]: https://raw.githubusercontent.com/GearHost/docs/master/Images/quick-glance.png
