#ASP Parent Paths
In classic .ASP you may find that parent paths are disabled in IIS on the GeaHost platform and you may see an error like the following.

    Active Server Pages error 'ASP 0131'
    Disallowed Parent Path
    /page/page.asp, line 2
    The Include file '../includes/something.asp' cannot contain '..' to indicate the parent directory.

Our advanced platform doesn't allow you to enable parent paths by default. You can however enable classic ASP parent paths on each CloudSite by creating a file named applicationHost.xdt and placing it in the CloudSite root /site folder using the code below.

> Please notice this is NOT the /site/wwwroot of your application but rather the /site folder off the root CloudSite for example /site/applicationHost.xdt.
    
    <?xml version="1.0"?>
    <configuration xmlns:xdt="http://schemas.microsoft.com/XML-Document-Transform">
      <system.webServer>
    <asp xdt:Transform="SetAttributes(enableParentPaths)" enableParentPaths="true" />
      </system.webServer>
    </configuration>
After you have added the code please make sure to fully stop your site fully, wait 10 seconds, then start your site back up. This should allow the application to fully stop and restart and then find the parent paths.
