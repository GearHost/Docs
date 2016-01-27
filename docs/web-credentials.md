#What is the publishing file?

***

CloudSites stores your FTP login information in a file called the publishing file.  You can download this file to get an automatically generated password assigned to your account when you create the application.   First you must login to your account and click the cloudsite you need the publishing information for. 

> Each application will have it's own publishing file and unique password.

![publish][publish-file]


####Publishing User Name
Your publishing user name will be the name of the application followed by \$ and then the name of the application again.  Here are a few examples as it is much easier to see than explain in words.

- CloudSite Application Name: example
- publishing user: example\$example

- Cloudsite Application Name: testapp
- Publishing User: testapp\$testapp


####publishing Password

Once you have downloaded the publishing file open it in any text editor and look for a line that says userPWD='' There will be a long password in the quotes to follow this field.  This is your application password and you can use it in combination with the publishing user name to log into your account via any ftp program.


> You will not need the quotation marks around the password in the userPWD='' field

##What is the the publishing file used for?
While you can use the details in side the publishing file to connect directly with a ftp program of your choice.  
You can use this publishing file with Visual Studio to authenticate to your site and publish with only a few clicks. You can also access the information in the document with a text editor to get the password and username to allow a user to have access to only that cloudsite rather than giving someone your deployment credentials, which have account wide permissions.

[publish-file]: https://raw.githubusercontent.com/GearHost/docs/master/Images/download-publishing-file.png