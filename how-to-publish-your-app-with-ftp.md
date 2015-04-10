#How to publish your application with FTP

Publishing your app using your favorite FTP client couldn't be easier wither GearHost. As with all FTP clients you will need the hostname, username and password. If you don't have a favoriate FTP client we recommend [FileZilla][filezilla-download].

###How is data stored on a CloudSite?
All data is tied to a particular CloudSite with each CloudSite having it's own individual login credentials. These credentials are used for FTP, Web Deploy and Git publishing. As such you need a specific individual login for each CloudSite you have.

###So where do I get that info?
1. To get your CloudSite login credentials to use for FTP (or Web Deploy and Git) you will need to [login to your GearHost account][login-link]
2. Click on the specific CloudSite you want to login info
3. Click on the Publish tab
4. Input the hostname, username and password info your FTP client and connect

This might look something like this:

Hostname: ftp.gear.host  
Username: myawesomeapp\$myawesomeapp  
Password: ydjcWguj0RamAJCbdjMtvzgxlkq3LJhuieblrY3sZeEiiuF6DRPZK8p3RMC6  

>Your username for FTP is the *{cloudsitename}*\$*{cloudsitename}* so if your CloudSite was called "myawesomeapp" your username would be "myawesomeapp\$myawesomeapp". FYI for Git your username is only $*{cloudsitename}* for example "$myawesomeapp".

>The password is very long and cannot be changed. This password cannot be changed however it can be reset and a new password generated for your CloudSite by clicking on the Reset Password button.

###Where do I put my data?
The web root content for your CloudSite is always located under /site/wwwroot.

###Using FileZilla?
If you are using FileZilla then we provide a downloadable XML file that you can import. Here's how to do it.

1. Download the FileZilla file by clicking on the icon in the GearHost control panel
2. Launch FileZilla
2. Under the File menu select Import
3. Select the file you downloaded
4. Select OK on the Import Settings dialog box
5. Select OK on the Import Successful confirmation box
6. Under the File menu select Site Manager or select the Site Manager icon
7. Under My Site select the CloudSite and click Connect

> You will need to enter your password again but you can select the "remember password" checkbox to save your password.

[filezilla-download]: https://filezilla-project.org/download.php?type=client
[Login-Link]:https://my.gearhost.com/account/login
 
