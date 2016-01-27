##Permission settings
On the Gearhost platform your applications do have full read and write permissions.
 A symptom of that you need to use relative pathing is if you are receiving an error such as
"Access to the path 'c:\inetpub\wwwroot\...' is denied.

##Relative pathing
c:\inetpub etc is not a valid path now on our managed hosting solution. You should access your files using relative pathing instead of absolute paths but if you do need to use an absolute path you can use c:\home as the prefix which drops you into your CloudSite application root. 

For example to get to the wwwroot of your CloudSite you would then use c:\home\site\wwwroot.


