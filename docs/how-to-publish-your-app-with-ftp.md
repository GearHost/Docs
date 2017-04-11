# Getting started with FTP

Publishing your app using your favorite FTP client couldn't be easier wither GearHost. As with all FTP clients you will need the hostname, username and password. If you don't have any FTP client installed, please be sure to check out our guide on installing Filezilla [here.](https://www.gearhost.com/documentation/installing-filezilla) 

### FTP credentials
1. Login to your hosting [portal](https://my.gearhost.com)
2. Click on your CloudSite
3. Select the **Publish** tab
4. Your information will be displayed below **"FTP Publishing Credentials"** 


It should look something like this:




    Hostname: ftp.gear.host  
    Username: yourcloudsitename\$yourcloudsitename  
    Password: S0M3RaV3RYjMtvL0NGLJhuiPA$$W0RDeEiiuF6DRPZK8p3RMC6


### Can I set my own password?
No, however it can be reset by clicking the **Reset Password** button on the right hand side.

### Can I create another FTP user?
At this time we do not support additional FTP accounts per CloudSite.

### Where do I upload my files?
The webroot directory for your CloudSite is **/site/wwwroot/**

### Import publishing file in Filezilla
We provide a XML file that you can import to Filezilla. This file saves your FTP connection to the Site Manager which makes it easier to connect. On the same **Publish** menu, click on the FileZilla icon to download the XML file.

1. Launch FileZilla
2. Under the **File** menu select **Import...**
3. Browse for the .xml file you just downloaded
4. Select OK on the Import Settings dialog box
5. Select OK on the Import Successful confirmation box
6. Under the **File** menu select **Site Manager**
7. Under **My Sites** select your CloudSite and click **Connect**


>**Tip:** If you're using Kudu or Git your username is $`yourcloudsitename` instead of `yourcloudsitename`\$`yourcloudsitename` If you're still having issues please open a [support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket) and we'll help you out!