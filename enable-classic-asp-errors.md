##Enable Classic ASP Errors

If you are having generic errors and can't figure out what the issue with your classic ASP site is you can enable Classic ASP errors. It's easy enough you just have to use the following code in your web.config to enable detailed errors. This is a great way to see issues although you will want to remove it once your site goes into production for security.

***

```<configuration>
<system.webServer>
    <httpErrors errorMode="Detailed" />
    <asp scriptErrorSentToBrowser="true"/>
</system.webServer>
<system.web>
    <customErrors mode="Off"/>
    <compilation debug="true"/>
</system.web>```
***