#How to configure PHP using .user.ini 

##Introduction
You can use a **.user.ini** file with your PHP application to configure PHP settings such as the amount of data that can be uploaded, displaying verbose errors, increasing memory limits, and many other configurations. A **.user.ini** file needs to be in the root of the application or website with the settings configured you wish to change. 

----------
This article covers several steps for configuring your PHP environment using `.user.ini`. The steps are:

1. [Create a .user.ini file](https://www.gearhost.com/documentation/how-to-configure-user-ini#user-content-creating-the-file)
2. [Memory Limit](https://www.gearhost.com/documentation/how-to-configure-user-ini#user-content-memory-limit)
3. [Max Upload Size](https://www.gearhost.com/documentation/how-to-configure-user-ini#user-content-max-upload-size)
4. [Max Execution Time](https://www.gearhost.com/documentation/how-to-configure-user-ini#user-content-max-execution-time)
5. [Max Input Time](https://www.gearhost.com/documentation/how-to-configure-user-ini#user-content-max-input-time)
6. [Max Post Size](https://www.gearhost.com/documentation/how-to-configure-user-ini#user-content-max-post-size)


----------


##Creating the file

1. Create a `.user.ini` file including the first period. Add the settings you want to change to the file using the same syntax as a php.ini. 
 
        ; Example Settings
    	display_errors=On
    	
2. Upload it to the root of your application or website. This is commonly the **/site/wwwroot/** directory.
 
3. [Restart your CloudSite](https://www.gearhost.com/documentation/restart-cloudsite) from the control panel. This forces the CloudSite to pull the new settings.

----------

##Memory Limit
This sets the maximum amount of memory in bytes that a script is allowed to allocate. This helps prevent poorly written scripts for eating up all available memory on a CloudSite.

`memory_limit = 256M`

##Max Upload Size
The maximum size of an uploaded file, this may required if you want to upload larger images or attachments.

`upload_max_filesize = 50M`


##Max Execution Time
This sets the maximum time in seconds a script is allowed to run before it is terminated by the parser. 

`max_execution_time=120`

##Max Input Time
This sets the maximum time in seconds a script is allowed to parse input data, like POST and GET.

`max_input_time=120`

##Max Post Size
Sets max size of post data allowed. This setting also affects file upload. 
To upload large files, this value must be larger than upload_max_filesize.

`post_max_size=1005M`

----------
**Tip:** You can create a PHP info page to view your current PHP values. We provide a guide on how to do that included [here.](https://www.gearhost.com/documentation/create-php-info-page)