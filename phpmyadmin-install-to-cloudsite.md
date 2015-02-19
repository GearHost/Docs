
##How to Install phpMyAdmin in a CloudSite

 
* Login to the control panel https://my.gearhost.com. 
* Create a new empty CloudSite. You may not be able to name it phpmyadmin as that name may be taken. You can name it anything you want though.
 
![step-1]
 
* Download the latest version of phpMyAdmin.

http://www.phpmyadmin.net/home_page/downloads.php
 
* Extract the files and upload them to your new CloudSite. Place all files in the wwwroot folder. 
* After the files have uploaded create a folder called config.

![step-2] 


 
* You'll need to gather the database information from the control panel. Navigate to Databases and click on the database you want to view. Scroll down and copy the address under database server. 

> Note: This will work with all your MySQL databases if they are on the same server. 

![step-3]

 
In the control panel go back to your CloudSite and launch it. You can use the launch button. 

![step-4]
 
* After it has launched add the subdirectory /setup/ to the end of the URL. For example if your URL is https://phpmyadmin.gear.host then you would type in https://phpmyadmin.gear.host/setup/.
> Note: Use https in front of the URL for a safer encrypted connection. 
* Click on the New Server button. 
* Type in the verbose name of the server, for example mysqlThen type in the address of the server in the hostname field. Leave everything else blank and click apply. 
* Click on download under the configuration file area. This will download the config file that then needs to be uploaded back into the wwwroot folder. 

![step-5]
 
* Upload the config.inc.php file to the wwwroot of your phpMyAdmin CloudSite. 
* After the file is uploaded delete the directories config and setup. 
* You can now login with your database user name and password. You can find this in the control panel under databases and then click on the database you wish to view. 

![step-6]
 
* Click on the eye ball to the far right to view the password. 

![step-7]
 
* When you launch the CloudSite you will see the login below. Enter the database information and click on go. 

![step-8]

[step-1]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-1.png
[step-2]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-2.png
[step-3]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-3.png
[step-4]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-4.png
[step-5]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-5.png
[step-6]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-6.png
[step-7]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-7.png
[step-8]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-8.png