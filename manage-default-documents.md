#Add and Update Default Documents

This article will cover how to add and arrange the default document that loads when a user visits your domain without specifying a file to load.

1. [What Is a Default Document?](https://www.gearhost.com/documentation/manage-default-documents#user-content-what-is-a-default-document)
2. [Manage your Default Documents](https://www.gearhost.com/documentation/manage-default-documents#user-content-manage-your-default-documents)
3. [Add a new default document](https://www.gearhost.com/documentation/manage-default-documents#user-content-add-a-new-default-document)
4. [Deleting unused Default Documents](https://www.gearhost.com/documentation/manage-default-documents#user-content-deleting-unused-default-documents)



***

##What Is a Default Document?
The Default document is used when you request a website on the internet from your browser that does not specify a document name. The default document specifies what file you would like to show your web visitors in this case.   

- www.gearhost.com <- **No document Specified**
- www.gearhost.com/my_cool_page.html <- my_cool_page.html is the document specified.

>Cloudsites comes configures with multiple default documents specified for the easy use it provides our customers. You can remove unneeded default documents for performance reasons.  

>You can also add your own custom default documents for instance if you wanted to show my_cool_page.html when someone visited your site without specifying that file name in the URL.


##Manage your Default Documents
 
[Log in to the control panel][Login-Link]

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
For each request, IIS must get the list of default documents and look for each file in the content path until it finds the first match. If you configure five documents and the site uses the last document, this increases the length of time spent that the system looks for the document. However, if you use one default document or use the first document in the list, this speeds up the request time.

You can click the small gray X next to any default document you do not wish to have in your list and it will not attempt to serve this content.  The pages listed are the standard pages that we add to each cloudsite and are not necessary if you are not using them.


[gearhost]: https://my.gearhost.com

[Login-Link]:https://my.gearhost.com/Account/Login


[default-documents]: https://raw.githubusercontent.com/GearHost/docs/master/Images/default-documents.png
[menu-cloudsites]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-cloudsites.png
[login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/login.png
[tab-config]: https://raw.githubusercontent.com/GearHost/docs/master/Images/tab-config.png
