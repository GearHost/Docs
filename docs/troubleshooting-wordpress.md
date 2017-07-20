# Troubleshooting WordPress
Having issues with your WordPress website? It can be multiple things, feel free to try one of the most common troubleshooting steps below.

## Enable PHP error debugging 
Create a `.user.ini` file and place it in your /site/wwwroot/. Add the following code and restart your CloudSite.
    
    error_reporting = E_ALL & ~E_DEPRECATED
    display_errors = On
    display_startup_errors = On

## Enable WP Debugging
To enable WordPress debugging insert these lines of code into your `wp-config.php`

    define('WP_DEBUG_LOG', true);
	define('WP_DEBUG_DISPLAY', false);
	define('SCRIPT_DEBUG', true);

**WP_DEBUG_LOG**: When WP_DEBUG_LOG and WP_DEBUG are enabled, WordPress saves all error information to the debug.log file in the wp-content directory. By default, this setting is disabled.

**WP_DEBUG_DISPLAY**: When WP_DEBUG_DISPLAY and WP_DEBUG are enabled, WordPress displays error and warning messages on web pages. By default, this setting is enabled. When this setting is disabled, debugging messages are hidden from view.

**SCRIPT_DEBUG**: When SCRIPT_DEBUG is enabled, WordPress uses development versions of core CSS and JavaScript files instead of the compressed versions that it normally uses. By default, this setting is disabled. You can use this setting to test modifications to built-in .js or .css files.

## Default Rewrite rules
You may have an issue with rewrite rules and may need the default rewrite rules.

    <?xml version="1.0" encoding="UTF-8"?>
    <configuration>
      <system.webServer>
    	<rewrite>
      	  <rules>
    		<rule name="wordpress" patternSyntax="Wildcard">
    		  <match url="*"/>
    			<conditions>
    				<add input="{REQUEST_FILENAME}" matchType="IsFile" negate="true"/>
    				<add input="{REQUEST_FILENAME}" matchType="IsDirectory" negate="true"/>
    			</conditions>
    		 <action type="Rewrite" url="index.php"/>
    		</rule>
		  </rules>
    	</rewrite>
      </system.webServer>
    </configuration>

## Before you start
The following queries will only work on default wordpress installations. We **HIGHLY recommend** to make a database backup before making changes. A guide can be found [here.](https://www.gearhost.com/documentation/how-to-backup-your-database) Connect to your Database remotely and run the following queries. If you don't know how to do this, please follow our documentation provided [here.](https://www.gearhost.com/documentation/connecting-to-mysql-database)

## Update Template
There may be an issue with your theme, so it's best to update these two tables to a default theme to determine if it's a theme issue or not.

    UPDATE `YOURDB`.`wp_options` SET `option_value` = 'THEMENAME' WHERE `wp_options`.`option_id` = 45;

## Update Stylesheet

    UPDATE `YOURDB`.`wp_options` SET `option_value` = 'THEMENAME' WHERE `wp_options`.`option_id` = 46;

## Disable all plugins
Sometimes it's plugins affecting your website, so it's best to disable all of them when troubleshooting.

    UPDATE `YOURDB`.`wp_options` SET `option_value` = 'a:0:{}' WHERE `wp_options`.`option_id` = 36;

## List WP Users

    SELECT * FROM YOURDB.wp_users;

It should display something like this, this will tell you which WP user belongs to which ID.

## Update your WordPress password
In this scenario we can see that ID=1 is "admin". This is how we would update the password for that user using MD5 encryption.
    
    UPDATE `YOURDB`.`wp_users` SET `user_pass` = MD5('YourNewPassWord') WHERE `wp_users`.`ID` = 1

Are you migrating your WordPress website? Maybe it has old URLs that require updating, here is the query on how to update your tables to the new url. Keep in mind that some images may be hardcoded to the old url and might require re-uploading.

## Update Site URL

    UPDATE `YOURDB`.`wp_options` SET `option_value` = 'http://yoursiteurl.com' WHERE `wp_options`.`option_id` = 1;

## Update Home URL

    UPDATE `YOURDB`.`wp_options` SET `option_value` = 'http://yoursiteurl.com' WHERE `wp_options`.`option_id` = 37;

## Contact forms
We recommend installing [Contact Form 7](https://wordpress.org/plugins/contact-form-7/) and  [WP-Mail-SMTP](https://wordpress.org/plugins/wp-mail-smtp/) plugins. After you're done configuring them, try testing your contact forms and see if it works.

>**Tip:** Still having issues? Please open a [support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket) and we can help you out!