#Support Article Template
***
*Target Platform:* Octane 
*Author:* Travis Haley 
*Created:* 10/26/2014  
*Version:* 1.0.1  
***
If after your review of this support article is you have any questions or feel something is not correct in this article please contact **support@gearhost.com** or tweet us **@GearHost**
***

##Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Install Wordpress](#1-install-wordpress)
4. [Update Wordpress Config](#2-update-wordpress-config)
5. [Change Style Files](#3-change-style-files)
6. [Tweaking Javascript](#4-tweaking-javascript)
7. [Conclusion](#conclusion)
8. [Supported Browsers](#supported-browsers)

***

##Introduction
This will be a small introduction to your article.  It should be a brief overview of what you are trying to explain however it should not go into any specific detail or steps to preform the task at hand.


##Prerequisites
This section will outline any prerequisites for completing this task.  It should include links to articles to preform the task if available:
 
* [Set up account](http://my.gearhost.com/login.aspx)
* [Set up FTP](http://support.gearhost.com/set-up-ftp)
* Download an FTP Client
    * [Filezilla](http://filezilla.com)
    * [Cute FTP](http://cuteftp.com)
* Additional Prerequisite 

***
##1. Install Wordpress
Details of step one:
 
* [download wordpress](http://www.wordpress.org)
* Connect via FTP
* Upload Wordpress to site
 
#####Download Wordpress
You will need to download wordpress from the main download site [here](http://wordpress.org)
#####Connect via FTP
Use the FTP client you downloaded in the prerequisites to connect to your account.
#####Upload Wordpress to site
Make sure the files go into your wwwroot folder. 
***

##2. Update Wordpress Config
This will be where you give a brief overview of step two (accessing wordpress admin):
 
* Update wp-config.php
* upload new wp-config.php
* connect to wp-admin
 
#####Update wp-config.php
1. On your local computer open the file wp-sample-config.php from the documents you downloaded.
2. update your connection string information from the database section of your cloudsite account.
3. save as wp-config.php (removing the sample from the filename)
#####upload new wp-config.php
after saving with the new filename connect with FTP and upload the new wp-config.php
#####connect to wp-admin
Browse to your-domain.com/wp-admin to connect for the first time.
***
##3. Change Style Files
 
To change these styles, go to the WordPress backend, select **Options > Styles** and select the style you would like.
***

##4. Tweaking Javascript
The content slider in the theme runs off of slider.js, and there are a couple of values that can be changed to alter the look and feel of the slider.

#####Changing Values
In slider.js, you can alter these values:
 
<code>auto: true</code>  
*Boolean: Animate automatically, true or false*  
 
<code>speed: 1000</code>  
*Integer: Speed of the transition, in milliseconds*
 
 
<code>pager: true</code>  
*Boolean: Show pager, true or false*  
 
<code>nav: false</code>  
*Boolean: Show navigation, true or false*  
***
##Conclusion
This would be a place to finalize any information you have provided.  Add any tips and tricks to this section as well.
***
##Supported Browsers 
This control panel feature works well (-) or great (X) in the following browsers:
 
**IE 6-8** -  
**IE 9+** X  
**Chrome** X  
**Firefox** X  
**Safari** X  
**Opera** X
***
####Support Documentation by
If you have any other questions that aren't covered in the documentation, feel free to e-mail <support@gearhost.com> or add a new post on the [forum](http://forum.gearhost.com/ "visit the forum").
