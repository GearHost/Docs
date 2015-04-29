Create a new CloudSite
==================

If you are developing a new website or application you will probably want to separate it from your others. You can do this by creating a new CloudSite. CloudSites are like containers that hold your application. A CloudSite also provides the resources necessary to run your application such as CPU cycles, memory, disk space, etc. It's recommended that you create a CloudSite for each application you are developing.  

>Add a new Cloudsite 

  1. After logging into your control panel click on CloudSites. 
 
  2. Click on the Add CloudSite button to begin adding a new CloudSite.
 
  3. Enter a site name. The site name will create a temporary URL that you can use to immediately launch the application or website and preview before changing DNS. The control panel will automatically check to see if the site name is being used somewhere else. If it is you will receive an error and will need to choose a new name.
 
   ![enter image description here](http://i.imgur.com/FyWVXnI.png)

  4. After choosing a site name you will need to choose a plan. 
 
- Free: The free plan is meant for developers. It is restricted in the amount of requests that can be made, memory use, and CPU use. This plan should not be used for any sort of production or public facing application or website. 
- Shared: This plan is not restricted like the free plan, but shares the resources of web servers in the cloud with other customers. However you are guaranteed a certain level of resources so your application cannot be impacted by others. 
- Reserved: This plan is unrestricted and gives you dedicated resources for your application or website.   
 
  ![enter image description here](http://i.imgur.com/YrlDPBH.png)

  5. After deciding on a plan you can choose to click on Create Empty CloudSite or Create CloudSite From Gallery. An empty CloudSite will simply build the resources you need without adding any files. If you already have an application choose empty CloudSite. If you would like to get started with a pre-built web application choose gallery and then choose the web app you wish to install. 
  6. After the CloudSite is built you will automatically be taken to the app within the control panel. From there you can configure your deployment credentials, download a publishing file, etc. 
