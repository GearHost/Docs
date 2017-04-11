# How to enable Directory Browsing


In this guide we will show you how to enable **Directory Browsing** for your application.



Edit your web.config file and add the following code:

    <configuration>
       <system.webServer>
    <directoryBrowse enabled="true" showFlags="Date,Time,Extension,Size" />
       </system.webServer>
    </configuration>


After making the change your application should display the list of files and should look something like this:


<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/directorybrowsing.PNG" />
