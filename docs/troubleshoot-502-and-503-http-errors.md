# Troubleshoot "502 bad gateway" and "503 service unavailable" HTTP errors
Every single application behaves differently, making it hard to determine what exactly is causing your application to fail. In this guide, we'll provide you with the basics steps required to begin troubleshooting your application.

### Why is it happening?
It may be due to the following: 

- Requests taking a long time
- Application using high memory/CPU
- Application crashing due to an exception

### What can be done to troubleshoot the error?
1. Configure [Site Diagnostics](https://www.gearhost.com/documentation/site-diagnostics#user-content-turning-logging-on-or-off) to enable `Web Server Logging` and `Detailed Error Messages`

2. Use the [Kudu Debug Console](https://www.gearhost.com/documentation/how-to-use-kudu) to troubleshoot your application


### What can be done to mitigate the issue?
We highly recommend to [scale](https://www.gearhost.com/documentation/how-to-scale-your-cloudsite) your application to the next tier plan. This will immediately add more CPU and RAM to your application, making it more powerful and less prone to crashing.

>**Tip:** Still stuck? Just [open a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket) and we'll be happy to help!