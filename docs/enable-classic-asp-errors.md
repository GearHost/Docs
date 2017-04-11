#  Enable Classic ASP Errors

If you would like your ASP scripts to show detailed errors rather than a generic error response this article will show you how to enable that. Simply create a new web.config file or modify your existing web.config file in your wwwroot folder to enable the scriptErrorSentToBrowser flag to true and existingResponse to PassThrough. Once done you may need to recycle your CloudSite by doing a stop then start to see the changes.

```
<?xml version="1.0" encoding="utf-8"?>
<configuration>
   <system.webServer>
		<asp scriptErrorSentToBrowser="true"/>
		<httpErrors existingResponse="PassThrough"/>
   </system.webServer>
</configuration>
```

> While this is useful please note this displays your raw error messages which may contain sensitive data. It is recommended to remove this after you have debugged the original issue.
