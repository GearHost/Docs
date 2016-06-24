#How to create a PHP Info page.

----------
Creating a [PHP Info](http://php.net/manual/en/function.phpinfo.php) provides the current PHP values that your application is loading. This can be convenient when making changes to `user.ini` and want to confirm if your changes are reflected.

----------


1. Create a file named `info.php`
	2. Place the following code in that file. 

		    <?php
		    
		    // Show all information, defaults to INFO_ALL
		    phpinfo();
		    
		    ?>

	3. Upload the file to your website's **/site/wwwroot/** directory.
	4. Visit `http://yourCloudSiteName.gear.host/info.php` or `http://yourdomain.com/info.php` on your browser.
	5. Look for the setting your changed such as the max file upload size and verify. It should display something like this: <img src="https://raw.githubusercontent.com/Gearhost/docs/master/Images/phpinfo.PNG" />


----------
**Tip:** Your `.user.ini` changes the **Local** value and that overrides the **Master** value.