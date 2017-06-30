# Always On

By default, CloudSite apps are unloaded if they are idle for a period of time. When **Always On** is enabled, it will automatically ping your app regularly to ensure it is always active and in a warm/running state. This is useful to ensure that a site is always responsive and that the worker process has not paged out due to lack of external HTTP requests. It is also useful as a way to keep a CloudSite active for scenarios when you want to run background code within it irrespective of whether it is actively processing external HTTP customer requests. This feature is only available on Small CloudSites or higher.

## Enabling Always On
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. **Select** your CloudSite
3. Click on the **Config** tab
4. Toggle the **Always On** button to enable this feature

![](https://raw.githubusercontent.com/GearHost/docs/master/Images/AlwaysOn.png)

>**Tip:**If you have any questions please let us know by [opening a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket).