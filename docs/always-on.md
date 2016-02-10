#Always On

By default, CloudSite apps are unloaded if they are idle for a period of time. When Always On is enabled on a CloudSite, Always On will automatically ping your app regularly to ensure it is always active and in a warm/running state. This is useful to ensure that a site is always responsive (and that the worker process has not paged out due to lack of external HTTP requests).

It is also useful as a way to keep a CloudSite active for scenarios when you want to run background code within it irrespective of whether it is actively processing external HTTP customer requests.

*Always On is a feature of Reserved mode CloudSite only.*

You can enable Always On support for a CloudSite by navigating to the CONFIG tab within a CloudSite, then toggling the Always On button:

![always-on]

[always-on]: https://raw.githubusercontent.com/gearhost/docs/master/docs/images/alwayson.png