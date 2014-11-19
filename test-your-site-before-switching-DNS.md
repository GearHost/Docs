How can you test your site before switching DNS
==================
***

##Preview URL Method
We provide you with an access domain name for every application in your control panel.  This access name is composed by your application name and gearhostcloud.com (example: myapplication.gearhostcloud.com) 

To find your access domain 

1. [Sign In to your account](my.gearhost.com)
2. Click on the CloudSite you wish to preview
 
![img1](http://i.imgur.com/1d68nli.png)
3. click on the launch CloudSite button in the upper right of the screen.

![img2](http://i.imgur.com/iPBEwSt.png)
You can visit sub folders for your site by adding them onto the end of the preview domain like any normal website folder.

##DNS bypassing using your HOSTS file
To test your website with your own domain name before DNS propagation has completed, you can use your local computer's HOSTS file. Your computer will use the entries in your HOSTS file before it looks up the DNS information for your domain. This article contains instructions for editing the HOSTS file on Windows 95/98/Me/2000/XP/2003/Vista/7/8/8.1, and Apple's Mac OS X.

When you are finished testing, remember to remove the custom lines that you added.

>**GearHost is not responsible for custom configurations on your local computer. If you are uncomfortable with editing configuration files on your computer, please do not follow the instructions below.**

####Windows
 1. Locate the HOSTS file on your local computer.  This is found in the following location in most default installations
  * Windows NT/2000/XP/2003/Vista/7 - C:\windows\system32\drivers\etc\hosts
  * Windows 95/98/Me - C:\windows\hosts
 2. Open the HOSTS file with a text editor such as Notepad or Wordpad
  * Right-click on Notepad and select the option to run Notepad as an Administrator as you need these elevated permissions to edit the HOSTS file.
  
 >**Consider performing a "Save As" so you have an original copy of the file that you can restore later.**

 You will see two columns of information, the first containing IP addresses and the second containing host names. By default, a windows hosts file should be similar to the following:

 ``` 127.0.0.1 localhost ```

 You can add additional lines to this file that will point requests for a resource to your new applications IP address

 ``` 
    127.0.0.1 localhost
    204.246.56.80 example.mysite.com
    204.246.56.80 mysite.com
    204.246.56.80 www.mysite.com
 ```
 
 3. Save your changes
 4. Restart any currently open web browsers on your local computer
 5. visit the site using the URL you added to your HOSTS
  * http://mysite.com
  * http://example.mysite.com
 



