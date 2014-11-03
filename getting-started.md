Getting Started 
==================

###Table of Contents
1. [Introduction](#user-content-introduction)
2. [Prerequisites](#user-content-prerequisites)
3. [Install Wordpress](#user-content-1-install-wordpress)
4. [Update Wordpress Config](#user-content-2-update-wordpress-config)
5. [Tweaking Javascript](#user-content-3-tweaking-javascript)
6. [Conclusion](#user-content-conclusion)
7. [Supported Browsers](#user-content-supported-browsers)

***

< iframe title="YouTube video player" width="480" height="390" src="http://www.youtube.com/watch?v=TheVideoID?autoplay=1" frameborder="0" allowfullscreen>< /iframe>

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

##3. Tweaking Javascript
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


