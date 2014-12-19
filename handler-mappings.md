How To Load Custom Handler Mappings
====

 There may be times when a Handler is not in IIS by default and you need to add the handler mapping to an application. This is now built in to the CloudSites Control Panel without the need to configure in IIS.

1. [Login to your account][login-link]

2. Navigate to the **CloudSites** Menu
 
    ![cloudsites][menu-cloudsites]

3. Open the **Config** tab

    ![scale][tab-config]
4. Scroll towards the bottom of this page until we see the following:

	![handler mapping][handler mapping]

5. In the first box we will set the file extension that will be associated with our Module

	![handler mapping][handler extension]

6. This next box will be the path to your Module. Once you are finished click **Save Configuration** at the bottom of your page to add the handler. Multiple handlers can be added by clicking **New Handler Mapping**.

	![handler mapping][handler path] 


[Login-Link]:https://my.gearhost.com/Account/Login


[menu-cloudsites]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-cloudsites.png
[login]: https://raw.githubusercontent.com/GearHost/docs/master/Images/login.png
[tab-config]: https://raw.githubusercontent.com/GearHost/docs/master/Images/tab-config.png
[handler mapping]: https://raw.githubusercontent.com/GearHost/docs/master/Images/handler-mapping.png
[handler extension]: https://raw.githubusercontent.com/GearHost/docs/master/Images/handler-mapping1.png
[handler path]: https://raw.githubusercontent.com/GearHost/docs/master/Images/handler-mapping2.png