Dot Net Nuke Quick Install 
==================

###Table of Contents
1. [Introduction](#user-content-introduction)
2. [Prerequisites](#user-content-prerequisites)
3. [Create CloudSite From Gallery](#user-content-1-creat-cloudsite-from-gallery)
4. [Install DNN](#user-content-2-install-dnn)
5. [Conclusion](#user-content-conclusion)
6. [Supported Browsers](#user-content-supported-browsers)

***

##Introduction
Here we will go over the steps to perform a quick install of Dot Net Nuke for your new CloudSite 

##Prerequisites
 
* [Set up account](http://my.gearhost.com/login.aspx)
* Standard SQL Plan or higher. Instructions for creating a database can be found [here](instrctions.com) 

***
##1. Create CloudSite From Gallery
Login to CloudSites:
 
* Create New CloudSite
* Select Installer

#####Create New CloudSite
You will need to create a New CloudSite for our Quick Installs. Instructions can be found [here](http://gearhostinstructions.com). Name your new CloudSite instance then select *Create CloudSite From Gallery* to install DNN using our Quick Install process.

#####Select Installer
Scroll on your left until you see the installer for DNN. Select by left clicking once, then clicking the check mark to the right of this window to continue 
***

##2. Install DNN
Now we will install and configure our Dot Net Nuke setup:
 
* Launch DNN Installer
* Configure DNN Setup
* 
 
#####Launch DNN Config Page
1. Once DNN is installed you will be taken to the front page of your new CloudSite.
2. Click Launch CloudSite to be taken to the DNN config page

#####Configure DNN Setup
1. *Administrative Information*: Create a username and password for your DNN admin page
2. *Website Information*: Name your website and select the template you wish to use with your DNN site. Here you will also select the language for your control panel
3. Database Information: Here we will connect the MSSQL database that we created for our DNN site. You will need the name of your database and the user credentials for this database in order to connect.
 * Select *Custom* under Database Setup
 * Database Type is *SQL Server/SQL Server Express Database*
 * *Server Name* will be the IP address for your SQL database
 * *Database Name* is the name of your database
 * At Security select *User Defined* and fill in the username and password for this database
 * Uncheck *Database Owner* under the *Run database as* option
 * Click **Continue** at the bottom of the screen

***
##Conclusion
After the installation you will be given the option to view your site and from here you can login to the DNN dashboard with the credentials you created earlier. You can access your admin dashboard anytime by visiting *yoursite*.gearhostcloud.com/admin 
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


