# MIME Types
In this article we will provide basic configuration for enabling MIME Types on your web.config. This file is usually placed in your /site/wwwroot/ if it doesn't exist it will require creating a new file.

##### Tip: SVG is already enabled by default, there's no need to enable it anymore.
If you were on a legacy environment and have been migrated to the new environment you might encounter an issue with SVG. We recommend using the following rule to resolve this issue in your **web.config.**

    <remove fileExtension=".svg" />
      <mimeMap fileExtension=".svg" mimeType="image/svg+xml"  />

##### Flash Player related
	<configuration>
	  <system.webServer>
		<staticContent>
			<remove fileExtension=".swf" />
			<mimeMap fileExtension=".swf" mimeType="application/x-shockwave-flash" />
		</staticContent>
	  </system.webServer>
	</configuration>

##### MP4/H264/Video related
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

##### Silverlight related
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

##### Graphics Interchange Format (GIF) related
	<configuration>
	  <system.webServer>
		<staticContent>
			<remove fileExtension=".gif" />
			<mimeMap fileExtension=".gif" mimeType="image/gif" />
		</staticContent>
	  </system.webServer>
	</configuration>

##### Joint Photographic Experts Group (JPEG) related
	<configuration>
 	   <system.webServer>
    	    <staticContent>
            	<remove fileExtension=".jpeg" />
            	<mimeMap fileExtension=".jpeg" mimeType="image/jpeg" />
				<remove fileExtension=".jpeg" />
            	<mimeMap fileExtension=".jpeg" mimeType="image/pjpeg" />
				<remove fileExtension=".jpg" />
            	<mimeMap fileExtension=".jpg" mimeType="image/jpeg" />
				<remove fileExtension=".jpg" />
            	<mimeMap fileExtension=".jpg" mimeType="image/pjpeg" />
        	</staticContent>
 	   </system.webServer>
	</configuration>


##### Portable Network Graphics (PNG) related
	<configuration>
 	   <system.webServer>
    	    <staticContent>
            	<remove fileExtension=".png" />
            	<mimeMap fileExtension=".png" mimeType="image/png" />
        	</staticContent>
 	   </system.webServer>
	</configuration>

##### JavaScript related
	<configuration>
 	   <system.webServer>
    	    <staticContent>
            	<remove fileExtension=".js" />
            	<mimeMap fileExtension=".js" mimeType="application/x-javascript" />
				<remove fileExtension=".js" />
            	<mimeMap fileExtension=".js" mimeType="application/javascript" />
				<remove fileExtension=".js" />
            	<mimeMap fileExtension=".js" mimeType="application/ecmascript" />
				<remove fileExtension=".js" />
            	<mimeMap fileExtension=".js" mimeType="text/javascript" />
				<remove fileExtension=".js" />
            	<mimeMap fileExtension=".js" mimeType="text/ecmascript" />
			</staticContent>
 	   </system.webServer>
	</configuration>

##### Text File related
	<configuration>
 	   <system.webServer>
    	    <staticContent>
            	<remove fileExtension=".txt" />
            	<mimeMap fileExtension=".txt" mimeType="application/octet-stream" />
        	</staticContent>
 	   </system.webServer>
	</configuration>

##### Portable Document Format (PDF) related
	<configuration>
 	   <system.webServer>
    	    <staticContent>
            	<remove fileExtension=".pdf" />
            	<mimeMap fileExtension=".pdf" mimeType="application/pdf" />
        	</staticContent>
 	   </system.webServer>
	</configuration>

##### Font WOFF, WOFF2, and Related
	<configuration>
 	   <system.webServer>
    	    <staticContent>
            	<remove fileExtension=".woff" />
            	<remove fileExtension=".woff2" />
            	<mimeMap fileExtension=".woff" mimeType="application/font-woff" />
            	<mimeMap fileExtension=".woff2" mimeType="application/font-woff2" />
        	</staticContent>
 	   </system.webServer>
	</configuration>