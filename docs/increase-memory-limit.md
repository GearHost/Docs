###Increasing memory limit for PHP

----------
By default PHP runs in a defined memory scope of 128M however if you are paying for a Standard CloudSite or Reserved you will want to increase this amount to 256M, 512M or even 1024M. The maximum allowed is 2048M on a Reserved CloudSite node. Increasing your PHP memory limit allows your PHP apps to run faster and with more stability. Below is how you can increase the PHP defined **memory_limit** value.



1. [Create a .user.ini file and place it in your /site/wwwroot folder](https://www.gearhost.com/documentation/php-user-ini)

1. Add the following code in .user.ini

    memory_limit = 512M

1. Restart your CloudSite and your new memory limit should start loading.

>[To verify your PHP settings create a phpinfo page](ddd)