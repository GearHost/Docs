PHP User.ini (Per site PHP ini settings)
==================

##Introduction
You can use a .user.ini file with your PHP application to configure some PHP environment settings such as the amount of data that can be uploaded or how to display errors. There are some settings that cannot be configured though. A .user.ini file needs to be in the root of the application or website with the settings configured you wish to change. 


##Per site ini settings
Anything in this list that is labeled `PHP_INI_ALL` or `PHP_INI_PERDIR` in the changeable can be changed in your .user.ini. [http://php.net/manual/en/ini.list.php](http://php.net/manual/en/ini.list.php)

Some examples of settings that are commonly changed. 

    ; Example Settings 
	; Default Value: E_ALL & ~E_NOTICE
	; Development Value: E_ALL | E_STRICT
	; Production Value: E_ALL & ~E_DEPRECATED
	; http://php.net/error-reporting   
    error_reporting = E_ALL & ~E_DEPRECATED

	; Default Value: On
	; Development Value: On
	; Production Value: Off
	; http://php.net/display-errors
    display_errors = On

	; Default Value: Off
	; Development Value: On
	; Production Value: Off
	; http://php.net/display-startup-errors
    display_startup_errors = On

	; Default Value: On
	; Development Value: Off
	; Production Value: Off
	; http://php.net/register-long-arrays
	register_long_arrays = Off
    
	; Maximum allowed size for uploaded files.
	; http://php.net/upload-max-filesize
	upload_max_filesize = 100M

	; Increase the amount of time allowed for a script to execute.
	max_execution_time = 10

	; Maximum size of POST data that PHP will accept.
	; http://php.net/post-max-size
	post_max_size = 10m

	; This sets the maximum amount of memory in bytes that a script is allowed to allocate.
	memory_limit = 64M

	; Default Value: On
	; Development Value: Off
	; Production Value: Off
	; http://php.net/magic-quotes-gpc
	magic_quotes_gpc = Off

`error_reporting` controls how errors are displayed. Change this to either show no errors or show detailed errors. Most of the time this will be configured to show no errors to hide sensitive information. 

`upload_max_filesize` will increase the maximum size of a file that can be uploaded to your site or app. Helpful for uploading large zip files or images.  

You can find more information on any setting you wish to change by googling it or using the [php manual](http://php.net/manual/en/). 

Settings that cannot be changed are also in that list. Look for anything in the changeable column labeled `PHP_INI_SYSTEM`.  

[http://php.net/manual/en/ini.list.php](http://php.net/manual/en/ini.list.php)
***
##Create the .user.ini file and upload it

1. Create a .user.ini file. Add the settings you want to change to the file using the same syntax as a php.ini. The file needs to be named `.user.ini` including the first period. 

        ; Example Settings
    	disaplay_errors=On
    	upload_max_filesize=10m

2. Upload it to the root of your application or website. In the screen shot below the file is in the wwwroot folder of my Wordpress site.

	![](http://i.imgur.com/2u48NNe.png)
 
3. Restart your CloudSite from the control panel. This forces the server to pull the new settings and override anything configured on the server level. 
4. Note: You can also use the [`ini_set()`](http://php.net/manual/en/function.ini-set.php) function in your scripts to configure individual settings. A .user.ini is easier since it creates a central location, but if there is one script you need to run longer you can set the max execution time higher on that single script for example.
5. After restarting you can verify the changes took place by creating a [php info](http://php.net/manual/en/function.phpinfo.php) file and running that from your app/site. 
	1. Create a file named info.php.
	2. Place the following code in that file. 

		    <?php
		    
		    // Show all information, defaults to INFO_ALL
		    phpinfo();
		    
		    // Show just the module information.
		    // phpinfo(8) yields identical results.
		    phpinfo(INFO_MODULES);
		    
		    ?>

	3. Upload the file to your account in the wwwroot folder. 
	4. Run the script on your site using the prefix URL GearHost provides yourCloudSiteName.gear.host or the FQDN of your CloudSite.
	5. Look for the setting your changed such as the max file upload size and verify. 


		![](http://i.imgur.com/4Avviju.png)

####Still need help?
If you have any other questions that aren't covered in this document, feel free to e-mail <help@gearhost.com>.