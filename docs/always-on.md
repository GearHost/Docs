#Always On

By default, CloudSite apps are unloaded if they are idle for a period of time. When Always On is enabled on a CloudSite, Always On will automatically ping your app regularly to ensure it is always active and in a warm/running state. This is useful to ensure that a site is always responsive and that the worker process has not paged out due to lack of external HTTP requests.

It is also useful as a way to keep a CloudSite active for scenarios when you want to run background code within it irrespective of whether it is actively processing external HTTP customer requests.

Always On is only available on Reserved CloudSites.

You can enable Always On support for a CloudSite by navigating to the Config tab of a CloudSite, then toggling the Always On button:

![](https://raw.githubusercontent.com/GearHost/docs/master/Images/AlwaysOn.png)

If you have any questions let us know and [open a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket).