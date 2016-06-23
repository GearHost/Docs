###Increasing memory limit for PHP

----------
Increasing your memory limit for PHP is important to get your plugins, themes, or scripts working properly. Below we will show you how to increase your **memory_limit**. By default a 128 mb limit is configured, but this can be easily updated to any limit you want depending on your CloudSite's plan. 

----------

1. Create a .user.ini file and place it in your root directory. If you already have one just add the following code. 


1. Add the following code in .user.ini

    memory_limit = 512M

1. Restart your CloudSite and your new memory limit should start loading.

----------
**Tip:** If you're unfamiliar with creating a .user.ini file we have a guide included [here](https://www.gearhost.com/documentation/php-user-ini) with more detailed steps.