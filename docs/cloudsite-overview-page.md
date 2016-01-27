CloudSite Overview
==================

*** 

##Introduction 
The Cloudsite Overview page provides general information regarding your CloudSite application.  You will find information about your CloudSite beginning with some resource stats. This page can also be used to configure your deployment credentials, grab your publishing file, and start and stop your CloudSite application among other things. 

*** 

##Access the Overview Page 



1. To access the Overview page [log in][login] to your control panel and then click on CloudSites from the left hand menu. 

    ![cloudsites][menu-cloudsites]

2. Now click on the CloudSite you wish to view the overview page for.
3. After choosing your CloudSite the first page you will see is Overview.

    ![overview][tab-overview]

***
##Dashboard  

 The first item you will see is a graph under dashboard giving you some current stats on your resources. This includes CPU time, data in and out, http errors, and requests. Below the graph you can change the amount of time it displays by clicking on 6 hours, 24 hours, or 7 days. Above the graph you can select what is displayed by unchecking or checking the different meters. For example I have only my requests and CPU time displayed for the last 6 hours because I have unchecked the other meters. 
 
 ![enter image description here](http://i.imgur.com/PnEpcS9.png)

 - CPU Time: This is the amount of time your application has used the CPU in a 24 hour period. GearHost allows 4 hours of CPU time in a 24 hour period for shared plans and 1 hour for free. Reserved plans are unlimited. Most websites will use far less than this. For example, my Wordpress site had 12,000 requests in 24 hours and only used 30 minutes of CPU time. 
 - Data In: This is the amount of data coming into your application, also known as bandwidth. Each time someone visits your website some data is sent to the GearHost cloud and processed by the web nodes. This information coming in is bandwidth. When a visitor uploads a file that would be data coming in as well. Free plans allow for 150MB per day, shared and reserved 1TB per month. 
 - Data Out: This is the amount of data your application sends out also known as bandwidth. Each time a visitor makes a request the GearHost cloud sends data to them whether they are on a desktop, tablet, or mobile phone. Images, code, java script, css, etc is all data that has to be given to the visitor. This data is bandwidth going out. Free plans allow for 150MB per day, shared and reserved 1TB per month. 
 - Http Errors: Any errors that are detected by the cloud. These could be script errors on the site, bad sessions, etc. We cannot display the exact error but if you are seeing a lot of them you can use debug tools and software to find the cause. You an also configure debug and logging options under the config page. Instructions can be found [here](https://www.gearhost.com/documentation/site-diagnostics).
 - Requests: Any time someone access yours application or website is a request. This does not correspond to visitors though because each visitor may make a few requests. That all depends on how your application or website is coded. 

***
##Usage Overview

 Below the graph is some helpful data displaying how many resources your application is consuming and how close that is to your plan limits. 

![](http://i.imgur.com/7IlBDne.png)

- CPU Time: Here the time is displayed as the percentage you have used of one hour. Remember shared accounts get 4 hours of CPU time in a 24 hour period. This is only showing how much you have used in one hour though. 
- Data Out: This is the amount of data you have sent out from your CloudSite, also known as bandwidth. For free plans this will be the amount for one day, for shared and reserved it will be a percentage of your total for the month. 
- File System Storage: Simply the amount of storage space you are consuming in the cloud. 
- Memory Usage: This is the amount of random access memory you consume in the cloud. The amount used all depends on how your application is programmed and also the programming language. For example .NET applications tend to cache more information in RAM than PHP applications do so a Wordpress site will often use less than a DotNetNuke site. 

***
##Quick Glance
Quick glance allows you to download your publishing file, reset it, and also set your deployment credentials. 

- Download Publishing File: This file can be used with visual studio, web matrix, or any other application that can read an xml publishing file. The publishing file contains the server address and credentials needed to publish code and content to your CloudSite. The credentials used are automatically configured for you to make it easier to publish. 
- Reset Publishing File: This simply resets the credentials. You may need this if you switch developers and want to prevent access for past developers. 
- Set Deployment Credentials: This configures a separate set of credentials that can be used for FTP or publishing if you are manually configuring an application to publish. 
- Start, Stop, Recycle: These buttons allow you to quickly stop your CloudSites, Start it back up, or recycle it. You'll often do this when publishing new code to refresh everything. It can also be used in troubleshooting or to bring the CloudSite down for maintenance. You'll see the page below when your CloudSite is stopped. 

    ![](http://i.imgur.com/haAe14E.png)
 
- Site URL: This is a quick way to get to your CloudSite without having to change and wait for DNS. It will always be yourCloudSiteName.gear.host.
- Status: The current status of your CloudSite, whether it is stopped or started. 
- Compute Mode: This represents the type of plan you have either free, shared, or reserved. 
- FTP Host Name: The server address to access your CloudSite through FTP. 
- Deployment / FTP User: The credentials used to access your CloudSite through FTP or deploy through various deployment tools like github.

####Still need help?
If you have any other questions that aren't covered in this documentation, feel free to e-mail <help@gearhost.com>.


[Login-Link]:https://my.gearhost.com/Account/Login

[menu-cloudsites]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-cloudsites.png
[login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/login.png
[tab-overview]: https://raw.githubusercontent.com/GearHost/docs/master/Images/tab-overview.png
