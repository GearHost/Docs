How to publish your app from visual studio 2013
==================

Below we'll walk through setting up deployment credentials and using those in Visual Studio 2013 to publish your application to your account. 

>Create your deployment credentials 

1. After logging into your control panel click on CloudSites and choose the site you want to publish to. 
 
2. Click on the button Download Publishing File.
 
3. The publishing file contains all of the information that Visual Studio will need to connect from your local computer to your cloudsite.  Open your solution and right click on the project name, then select publish.  *Your site cannot be running in debug for this option to appear.*
 
 ![publish settings](http://i.imgur.com/mhyukAo.png)

4. Click on Import to import the publishing file you downloaded in step two.

 ![import](http://i.imgur.com/DkqAiQy.png)  

5. Click Browse and locate the downloaded file on your hard drive. Then click OK

 ![Imgur](http://i.imgur.com/13MwSSg.png)

6. All of the publishing information will be filled in automatically for you.  You can validate connection or just click publish. *this will upload all of your site files from your local source project to the cloudsite*

 ![Imgur](http://i.imgur.com/whY0G7b.png)
  


 

