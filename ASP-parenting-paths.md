#ASP parent paths
In classic .ASP you may find that parent paths are disabled in IIS on the GeaHost platform and you may see an error like the following.

    Active Server Pages error 'ASP 0131'
    Disallowed Parent Path
    /page/page.asp, line 2
    The Include file '../includes/something.asp' cannot contain '..' to indicate the parent directory.

Our advanced platform doesn't allow you to enable parent paths. However the applicationhost.config can be changed per your instance. If you need to enable parent paths for ASP you will need to add the following to your applicatiohost.config. 
    
    <?xml version="1.0"?>
    <configuration xmlns:xdt="http://schemas.microsoft.com/XML-Document-Transform">
      <system.webServer>
    <asp xdt:Transform="SetAttributes(enableParentPaths)" enableParentPaths="true" />
      </system.webServer>
    </configuration>

