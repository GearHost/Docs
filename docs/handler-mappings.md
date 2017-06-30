# Enable Custom Extensions in The Default PHP Run Time
By default, PHP 5.4 is installed and immediately available for use when you create an Azure Website. The best way to see the available release revision, its default configuration, and the enabled extensions is to deploy a script that calls the phpinfo() function.

>Save this a phpinfo.php and upload to your wwwroot

```<?php
phpinfo();
?>
```

The best way to see the default PHP version, its default configuration, and the enabled extensions is to deploy a script that calls phpinfo(). To enable additional extensions, follow the steps below.

Add a bin directory to your root directoy.
Put .dll extension files in the bin directory (for example, php_mongo.dll). Make sure that the extensions are compatible with default version of PHP (which is, as of this writing, PHP 5.4) and are VC9 and non-thread-safe (nts) compatible.
Deploy your application.
Navigate to your site's dashboard in the Azure Portal, and click on Configure.

Configure tab on Web Sites dashboard

In the app settings section, create a key PHP_EXTENSIONS and a value bin\your-ext-file. To enable multiple extensions, incude a comma-separated list of .dll files.

Enable extension in app settings

Click Save at the bottom of the page.

Save configuration settings

1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)

3. Open the **Config** tab
    ![scale][tab-config]

4. Scroll towards the bottom of this page until we see the following:
	![handler mapping][handler mapping]

5. In the first box we will set the file extension that will be associated with our Module
	![handler mapping][handler extension]

6. This next box will be the path to your Module. Once you are finished click **Save Configuration** at the bottom of your page to add the handler. Multiple handlers can be added by clicking **New Handler Mapping**.
	![handler mapping][handler path] 

[menu-cloudsites]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-cloudsites.png
[login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/login.png
[tab-config]: https://raw.githubusercontent.com/GearHost/docs/master/Images/tab-config.png
[handler mapping]: https://raw.githubusercontent.com/GearHost/docs/master/Images/handler-mapping.png
[handler extension]: https://raw.githubusercontent.com/GearHost/docs/master/Images/handler-mapping1.png
[handler path]: https://raw.githubusercontent.com/GearHost/docs/master/Images/handler-mapping2.png