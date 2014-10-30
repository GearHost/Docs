How to publish your app with FTP on OSX
==================

Below we'll walk through setting up deployment credentials and using those in an FTP client to publish your application to your account. 

>Create your deployment credentials 

 1. After logging into your control panel click on CloudSites and choose the site you want to publish to. 
 
 2. Click on the button Set Deployment Credentials.
 
 3. Type in a user name and password you would like to use and click change password. *It's important to note that your deployment credentials are used for all your CloudSites. When you set or change them on one CloudSite it will change the password for your other CloudSites. Each CloudSite will have a different user name though.* 
 
 4. Now that you have your credentials you can enter them into an FTP client like [FileZilla](https://filezilla-project.org/download.php?type=client). You can find the server address on the same page in the control panel as where you configured your deployment credentials, ftp.gearhostcloud.com. Your user name is also there. *Note that the user name includes your CloudSite name. In the example below "example1" is the name of my CloudSite, "ftpuser1" is the user I created for deployment. Each CloudSite will ...(line truncated)...
 
 ![enter image description here](http://i.imgur.com/G4ifdqG.png)


 
> Enter your credentials in FileZilla
 

 1. Open FileZilla and in the quick connect bar enter the server, user name, and password. Remember you can find the information on the Overview page of your CloudSite in your control panel.
 
 ![enter image description here](http://i.imgur.com/WSXYvMe.png)
 
 2. Click Quickconnect and you will be connected to the FTP server. 
 
 3. Now you will be able to upload your app

>Alternative Method Using Finder
>

 1. Open a new Finder window
 2. Select *Go* from the Menu Bar then select *Connect to Server*
 
  ![Imgur](http://i.imgur.com/1U9IuI4.png)

 3.Enter the CloudSites FTP server address in the *Server Address* bar
  ![Imgur](http://i.imgur.com/6wDwy4f.png)
  
 4. Enter the credentials created earlier for your CloudSite the select *Connect*. Once connected, your folders will open in a separate window and you can click and drag files to your FTP server
  ![Imgur](http://i.imgur.com/iNm0yPu.png)
