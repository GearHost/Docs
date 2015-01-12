Add and Update Default Documents
==================

This article will cover how to add and arrange the default document that loads when a user visits your domain without specifying a file to load.

***
##1. Manage your Default Documents
 
[Log in to the control panel][Login-Link]

![login][login]

#####Click on CloudSites
Once logged in click on CloudSites and then choose your CloudSite.

![cloudsites menu][menu-cloudsites]

#####Click on the Config tab.
After you choose your CloudSite click on the config tab. 

![config][tab-config]

##Add a new default document

At the bottom of the Default Documents section inside of the config panel we reached in the above steps there is a button for New Default Document

>It is important to note that the web server will look at these in order so any document nearest the top will be served on down the list to the bottom.

If you need to raise a site higher in the document list you can cut and paste the document you need higher into the top spot.  We recommend using the top spot for your main default document that you will be using.  This will be based on your programming language.

![default documents][default-documents]

##Deleting unused Default Documents
You can click the small gray X next to any default document you do not wish to have in your list and it will not attempt to serve this content.  The pages listed are the standard pages that we add to each cloudsite and are not necessary if you are not using them.


[gearhost]: https://my.gearhost.com

[Login-Link]:https://my.gearhost.com/Account/Login


[default-documents]: https://raw.githubusercontent.com/GearHost/docs/master/Images/default-documents.png
[menu-cloudsites]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-cloudsites.png
[login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/login.png
[tab-config]: https://raw.githubusercontent.com/GearHost/docs/master/Images/tab-config.png
