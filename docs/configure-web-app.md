#Configure Web Apps
This article explains how to configure a web app using the Octane configuration menu.

##General Settings
Framework versions. Set these options if your app uses any these frameworks:

**.NET Framework version:** Set the .NET framework version. **v3.5** supports *2.0, 3.0, 3.5,* and *3.5.1*. **v4.6** supports *4.0, 4.5, 4.5.1-2, 4.6, and 4.6.1-2*

**PHP Version:** Set the PHP version, or OFF to disable PHP. We currently support 5.3, 5.4 and 5.5.

**Managed Pipeline Version:** Sets the IIS pipeline mode. Leave this set to **Integrated** (the default) unless you have a legacy app that requires an older version of IIS.

**Web Sockets:** Set **ON** to enable the WebSocket protocol; for example, if your web app uses [ASP.NET SignalR](http://www.asp.net/signalr) or [socket.io.](https://azure.microsoft.com/en-us/documentation/articles/web-sites-nodejs-chat-app-socketio/) Web Sockets requires a Standard CloudSite or higher.

**Platform:** Selects whether your web app runs in a 32-bit or 64-bit environment. The 64-bit environment requires a Standard CloudSite or higher. 

**Always On:** By default, web apps are unloaded if they are idle for some period of time. This lets the system conserve resources. Only in a Reserved CloudSite or higher, you can enable **Always On** to keep the app loaded all the time. If your app runs continuous web jobs, you should enable **Always On**, or the web jobs may not run reliably.


##Site Diagnostics
**Web Server Logging:** Logs are saved in the W3C extended log file format.

**Detailed Error Messages:** Saves detailed error messages .htm files. The files are saved under /LogFiles/DetailedErrors.

##App Settings
This section contains name/value pairs that you web app will load on start up.

1. For .NET apps, these settings are injected into your .NET configuration `AppSettings` at runtime, overriding existing settings.

1. PHP and Node applications can access these settings as environment variables at runtime. For each app setting, two environment variables are created; one with the name specified by the app setting entry, and another with a prefix of APPSETTING_. Both contain the same value.

<img src="https://raw.githubusercontent.com/Gearhost/docs/master/Images/relic3.PNG" />

##Connection strings
Connection strings for linked resources.

For .NET apps, these connection strings are injected into your .NET configuration connectionStrings settings at runtime, overriding existing entries where the key equals the linked database name.

For PHP and Node applications, these settings will be available as environment variables at runtime, prefixed with the connection type. The environment variable prefixes are as follows:

SQL Server: `SQLCONNSTR_`

MySQL: `MYSQLCONNSTR_`

Custom: `CUSTOMCONNSTR_`

For example, if a MySQL connection string were named `connectionstring1`, it would be accessed through the environment variable `MYSQLCONNSTR_connectionString1`.

##Default Documents
The default document is the web page that is displayed at the root URL for a website. The first matching file in the list is used. Web apps might use modules that route based on URL, rather than serving static content, in which case there is no default document as such.

##Handler Mappings
Use this area to add custom script processors to handle requests for specific file extensions.

**Extension:** The file extension to be handled, such as *.php or handler.fcgi.

**Script Processor Path** The absolute path of the script processor. Requests to files that match the file extension will be processed by the script processor. Use the path \home\site\wwwroot to refer to your app's root directory.

**Additional Arguments:** Optional command-line arguments for the script processor.


##Virtual Directories
To configure virtual applications and directories, specify each virtual directory and its corresponding physical path relative to the website root. Optionally, you can select the Application checkbox to mark a virtual directory as an application.

>**Tip:** If you ever need assistance or clarification on anything please [open a support ticket.](https://www.gearhost.com/documentation/how-to-open-a-support-ticket)