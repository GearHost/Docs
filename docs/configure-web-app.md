# CloudSite - Configure menu
In this article we go over the basic configurations you can enable on your CloudSite. This great feature allows each CloudSite to be individually customized and run on their own custom environment separately!

#  General Settings
Framework versions. Set these options if your app uses any these frameworks:

1. **.NET Framework version:** Set the .NET framework version.
 Version `3.5` supports 2.0, 3.0, and 3.5.
 Version `4.6` supports 4.0, 4.5, 4.5, 4.6, and 4.6

2. **PHP Version:** Set the PHP version, or toggle `OFF` to disable PHP. We currently support versions; `5.3`, `5.4`, `5.5`, and `7`.

3. **Managed Pipeline Version:** Sets the IIS pipeline mode. By default it's on `Integrated` mode, but you can also select `Classic` which is recommend for some legacy apps. 

4. **Web Sockets:** Set `ON` to enable the WebSocket protocol. This is recommended if your app uses [ASP.NET SignalR](http://www.asp.net/signalr) or [socket.io.](https://azure.microsoft.com/en-us/documentation/articles/web-sites-nodejs-chat-app-socketio/) Please note that this feature is only available on Hobby CloudSites or higher.

6. **Platform:** You can toggle your app's mode to be `32-bit` or `64-bit`. Please note that 64-bit mode is only available on Hobby CloudSites or higher. Also, PHP 7 now supports 64-bit applications.

7. **Always On:** By default, web apps are unloaded if they are idle for some period of time. This lets the system conserve resources. On a Small node or higher, you can enable `Always On` to keep your app always active. If your app runs continuous web jobs, you should enable `Always On` or the web jobs may not run reliably.


#  Site Diagnostics
**Web Server Logging:** Logs are saved in the W3C extended log file format.

**Detailed Error Messages:** Saves detailed error messages .htm files. The files are located in */LogFiles/DetailedErrors/*.

#  App Settings
This section contains name/value pairs that you web app will load on start up.

1. For .NET apps, these settings are injected into your .NET configuration `AppSettings` at runtime, overriding existing settings.

1. PHP and Node applications can access these settings as environment variables at runtime. For each app setting, two environment variables are created; one with the name specified by the app setting entry, and another with a prefix of `APPSETTING_`. Both contain the same value.

<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/php-zend-extensions.PNG" />

#  Connection strings
Connection strings for linked resources.

For .NET apps, these connection strings are injected into your .NET configuration connectionStrings settings at runtime, overriding existing entries where the key equals the linked database name.

For PHP and Node applications, these settings will be available as environment variables at runtime, prefixed with the connection type. The environment variable prefixes are as follows:

SQL Server: `SQLCONNSTR_`

MySQL: `MYSQLCONNSTR_`

Custom: `CUSTOMCONNSTR_`

For example, if a MySQL connection string were named `connectionstring1`, it would be accessed through the environment variable `MYSQLCONNSTR_connectionString1`.

#  Default Documents
The default document is the web page that is displayed at the root URL for a website. The first matching file in the list is used. Web apps might use modules that route based on URL, rather than serving static content, in which case there is no default document as such.

#  Handler Mappings
Use this area to add custom script processors to handle requests for specific file extensions.

**Extension:** The file extension to be handled, such as *.php or handler.fcgi.

**Script Processor Path** The absolute path of the script processor. Requests to files that match the file extension will be processed by the script processor. Use the path *\home\site\wwwroot* to refer to your app's root directory.

**Additional Arguments:** Optional command-line arguments for the script processor.


#  Virtual Directories
To configure virtual applications and directories, specify each virtual directory and its corresponding physical path relative to the website root. Optionally, you can select the Application checkbox to mark a virtual directory as an application.

>**Tip:** If you ever need assistance or clarification on anything please [open a support ticket.](https://www.gearhost.com/documentation/how-to-open-a-support-ticket)