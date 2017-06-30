# URL Rewrites and Redirects
This guide will go over enabling URL rewrites or setting up redirects for your domain.

**What is a URL Rewrite?**

It's a function that automatically adds **https://** or **www.** after someone visits **domain.com**.
Thus, making your domain load the SSL immediately or making it look like **http://www.domain.com**

### web.config
You will have to modify your web.config. 
If this file does not exist, create one inside your root directory.

**HTTP to HTTPS rewrite**

This rule will enable your SSL to load when someone visits your domain. If you're using a CMS, it's likely that you will have to enable that function within its panel instead.

    <?xml version="1.0" encoding="UTF-8"?>
    <configuration>
      <system.webServer>
    <rewrite>
      <rules>
    <rule name="HTTP to HTTPS redirect" stopProcessing="true">
      <match url="(.*)" />
    <conditions>
      <add input="{HTTPS}" pattern="off" ignoreCase="true" />
    </conditions>
      <action type="Redirect" redirectType="Found" url="https://{HTTP_HOST}/{R:1}" />
    </rule>
      </rules>
    </rewrite>
      </system.webServer> 
    </configuration> 

**Non-WWW to WWW rewrite**

This rule will enable WWW. on your domain.

    <?xml version="1.0" encoding="UTF-8"?>
    <configuration>
      <system.webServer>
    <rewrite>
      <rules>
    <rule name="Redirect to WWW" stopProcessing="true">
      <match url=".*" />
      <conditions>
    <add input="{HTTP_HOST}" pattern="^YOURDOMAIN.COM$" />
      </conditions>
      <action type="Redirect" url="http://www.YOURDOMAIN.COM/{R:0}"
      redirectType="Permanent" />
    </rule>
      </rules>
    </rewrite>
      </system.webServer>  
    </configuration>
    
**Redirect to destination url**

This rule will make your domain.com redirect to any other domain you want.
    
    <?xml version="1.0" encoding="UTF-8"?>
    <configuration>
      <system.webServer>
    <rewrite>
      <rules>
    <rule name="Redirect to another url" stopProcessing="true">
      <match url=".*" />
      <conditions>
    <add input="{HTTP_HOST}" pattern="^yourdomain.com$" />
      </conditions>
      <action type="Redirect" url="http://www.destinationurl.com/{R:0}"
      redirectType="Permanent" />
    </rule>
      </rules>
    </rewrite>
      </system.webServer> 
    </configuration>

### HTML redirect to destination url
Alternatively, you can use HTML to redirect if that's easier for you.

    <meta http-equiv="refresh" content="0; url=http://destinationurl.com/" />

### Redirect page to directory
You can create url redirects to load a certain directory instead. 

    <rules>	
    	<rule name="about to about directory" stopProcessing="true">
    <match url="aboutus.asp" />
    <action type="Redirect" url="/home/about" appendQueryString="true" />
    				</rule>
    			</rules>

>**Tip:** If you're creating multiple redirect rules in your web.config be sure to create a different rule name for each one.