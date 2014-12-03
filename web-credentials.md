##What is the publishing file?
***
![publish][publish-file]

Publishing files are site specific credentials. You can extract your user password for this specific site by accessing the file with a text editing program. You password will follow userPWD=. You will not need the quotation marks. Your username is also listed here, however it will always be $sitename. 

##What is the the publishing file used for?
You can use this file with Visual Studio to authenticate to your site and publish. You can also access the information in the document with a text editor to get the password and username to allow a user to have access to only that cloudsite rather than giving someone your deployment credentials, which have account wide permissions.

[publish-file]: https://raw.githubusercontent.com/GearHost/docs/master/Images/download-publishing-file.png