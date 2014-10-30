Git Deploying Your Application
==================

###Table of Contents
1. [Introduction](#user-content-introduction)
2. [Prerequisites](#user-content-prerequisites)
3. [Installing and Configuring Git](#user-content-1-Installing-and-Configuring-Git)
4. [Initialize a Git repository for your application](#user-content-2-Initialize-a-Git-repository-for-your-application)
5. [Deploy Application to CloudSite](#user-content-3-Deploy-Application-to-cloudsite)
6. [Additionsl Resources](#user-additional-resources)
7. [Supported Platforms](#user-content-supported-platforms)

***

##Introduction
The content in this article covers deploying an application or website from a Git repository.  We also support online Git repositories like [GitHub](http://github.com) and [BitBucket](http://bitbucket.com) it your team is using a cloud based deployment solution.


##Prerequisites
You must have an account set up and your email verification complete to use the cloudsite application install gallery:
 
* [Set up account](http://my.gearhost.com/login.aspx)

***
##1. Installing and Configuring Git
*You do not need to do this step if you already have Git installed on your local computer*

 
* [download Git](http://git-scm.com/download/)
* Install Git
* Configure Git
 
#####Download Git
You will need to download Git from the main download site [here](http://wordpress.org)
#####Connect via FTP
Use the FTP client you downloaded in the prerequisites to connect to your account.
#####Upload Wordpress to site
Make sure the files go into your wwwroot folder. 
***

##2. Initialize a Git repository for your application
This will be where you give a brief overview of step two (accessing wordpress admin):
 
* Commit your local files
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

##3. Deploy Application to your CloudSite
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
##Additional Resources
This would be a place to finalize any information you have provided.  Add any tips and tricks to this section as well.
***
##Supported Platforms 
Git Deploy is available for the following operating systems:
 
**Windows**   
**Linux**  
**Mac** 



