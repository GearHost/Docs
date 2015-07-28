
##How to Install phpMyAdmin in a CloudSite

####This guide is for a simple phpMyAdmin setup and it's not recommended for any custom/advanced phpMyAdmin settings.



* Login to the control panel https://my.gearhost.com. 
* Create a new empty CloudSite. You may not be able to name it phpMyAdmin as that name may be taken. You can name it anything you want though.
 
![step-1]
 
* Download the latest version of phpMyAdmin.

http://www.phpmyadmin.net/home_page/downloads.php
 
* Extract the files and upload them to your new CloudSite. Place all files in the wwwroot folder. 

![step-2] 


 
* You'll need to gather the database information from the control panel ( https://my.gearhost.com/Databases ).  Click on the database you want to view. This will provide the server it's currently hosted on.



![step-3]

 

 
* Download the following file: [config.inc.php](https://raw.githubusercontent.com/GearHost/docs/master/files/config.inc.php) . It's pre-configured to connect to our MySQL servers.
* Open the config.inc.php and update the keyword "PLEASEUPDATEME" on line 17 to any random letters & numbers. This would be for cookie encryption. It can be something such as "123651b1561d891651" then save the file. 
* Upload config.inc.php to the wwwroot of your phpMyAdmin CloudSite. 
* After the file is uploaded delete the "setup" directory and "config.sample.inc.php" file.

In the control panel go back to your CloudSite and launch it. You can use the launch button. 


![step-5]

* You can now login with your database user name and password as well as select which MySQL server you wish to connect to. 
![step-9]

* You can find this in the control panel under databases and then click on the database you wish to view. 

![step-6]
 
* Click on the eye ball to the far right to view the password. 

![step-7]
 
* When you launch the CloudSite you will see the login below. Enter the database information and click on go. 

![step-8]

[step-1]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-1.png
[step-2]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-2.png
[step-3]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-3.png
[step-5]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-5.png
[step-6]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-6.png
[step-7]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-7.png
[step-8]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-8.png
[step-9]: https://raw.githubusercontent.com/GearHost/docs/master/Images/phpmyadmin-9.png