# Troubleshooting WordPress
Having issues with your WordPress website? It can be multiple things, feel free to try one of the most common troubleshooting steps below.

## Enable PHP error debugging 
Create a **.user.ini** file and place it in your /site/wwwroot/. Add the following code and restart your CloudSite.
    
    error_reporting = E_ALL & ~E_DEPRECATED
    display_errors = On
    display_startup_errors = On

## Enable WP Debugging
On your wp-config.php file there should be a line "WP_debug" set that to true.

    define('WP_DEBUG', true);

## Web.config
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
    			</rule></rules>
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
![wpusers](https://raw.githubusercontent.com/GearHost/docs/master/Images/wp_users_db_table.PNG)

## Update your WordPress password
In this scenario we can see that ID=1 is "monroykid". This is how we would update the password for that user using MD5 encryption.
    
    UPDATE `YOURDB`.`wp_users` SET `user_pass` = MD5('YourNewPassWord') WHERE `wp_users`.`ID` = 1

Are you migrating your WordPress website? Maybe it has old URLs that require updating, here is the query on how to update your tables to the new url. Keep in mind that some images may be hardcoded to the old url and might require re-uploading.

## Update Site URL

    UPDATE `YOURDB`.`wp_options` SET `option_value` = 'http://yoursiteurl.com' WHERE `wp_options`.`option_id` = 1;

## Update Home URL

    UPDATE `YOURDB`.`wp_options` SET `option_value` = 'http://yoursiteurl.com' WHERE `wp_options`.`option_id` = 37;

## Contact forms
We recommend installing [Contact Form 7](https://wordpress.org/plugins/contact-form-7/) and  [WP-Mail-SMTP](https://wordpress.org/plugins/wp-mail-smtp/) plugins. After you're done configuring them, try testing your contact forms and see if it works.

>**Tip:** Still having issues? Please open a [support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket) and we can help you out!