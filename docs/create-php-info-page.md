# Create a PHP Information Page

Creating a [PHP Info Page](http://php.net/manual/en/function.phpinfo.php) provides the current PHP values that your application is loading. This can be convenient when making changes to the [.user.ini](https://www.gearhost.com/documentation/how-to-configure-user-ini) and want to confirm your PHP configuration.


1. Create a file named **info.php** and upload it in */site/wwwroot/*

1. Place the following code in that file

			<?php phpinfo(); ?>
	
1. After your changes have been saved, you can visit `http://{yourcloudsite}.gearhostpreview.com/info.php` or `http://{yourdomain.com}/info.php` to view your PHP output.
	
> **Tip**: Trying to enable PHP debugging? We show an example on how to do this [here](https://www.gearhost.com/documentation/troubleshooting-wordpress#user-content-enable-php-error-debugging)!