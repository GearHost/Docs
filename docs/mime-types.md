##MIME Types

----------

In this article we will provide basic configuration for enabling MIME Types on your web.config. This file is usually placed in your /site/wwwroot/ if it doesn't exist it will require creating a new file.

#####Tip: SVG is already enabled by default, there's no need to enable it anymore.

----------

If you were on a legacy environment and have been migrated to the new environment you might encounter an issue with SVG. We recommend using the following rule to resolve this issue in your **web.config.**

    <remove fileExtension=".svg" />
      <mimeMap fileExtension=".svg" mimeType="image/svg+xml"  />

#####MP4/H264/Video related
    
     <configuration>
    <system.webServer>
	<staticContent>
            <remove fileExtension=".mp4" />
            <mimeMap fileExtension=".mp4" mimeType="video/mp4" />
            <remove fileExtension=".m4v" />
            <mimeMap fileExtension=".m4v" mimeType="video/m4v" />
        </staticContent>
		</system.webServer>
    </configuration>

#####Silverlight related

    <configuration>
    <system.webServer>
        <staticContent>
			 <remove fileExtension=".xaml" /> 
             <mimeMap fileExtension=".xaml" mimeType="application/xaml+xml" />
			 <remove fileExtension=".xap" />
             <mimeMap fileExtension=".xap" mimeType="application/x-silverlight-app" />
			 <remove fileExtension=".xbap" />
             <mimeMap fileExtension=".xbap" mimeType="application/x-ms-xbap" />
         </staticContent>
    </system.webServer>
    </configuration> 