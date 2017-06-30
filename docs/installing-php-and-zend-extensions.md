# Installing PHP and Zend Extensions on a CloudSite
This article covers two steps needed to install custom PHP and Zend extensions for use with your CloudSite application. This article will demo installing two extensions.  one being MongoDB a regular extension and the second IonCube a Zend extension. The steps are:

1. [Download and Upload the extensions](https://www.gearhost.com/documentation/installing-php-and-zend-extensions#user-content-download-and-upload-the-extensions)
2. [Configure the CloudSite from your portal to load the extensions](https://www.gearhost.com/documentation/installing-php-and-zend-extensions#user-content-configure-the-cloudsite-from-your-portal-to-load-the-extensions)

## Download and Upload the extensions
1. Download the appropriate extension that you wish to run with your application
2. Create a folder called **bin** under the **/site/wwwroot** using any FTP client

> It is important you download the appropriate version of the extension you are intending to run.  by default the CloudSite will run in **32 bit** mode unless changes in your configuration.  You should also download **Non Thread Safe** versions of your extension if available.

## Configure the CloudSite from your portal to load the extensions
1. [Log in to your GearHost Account][login-link]
2. Click on the CloudSite menu option if not already active
3. Select your CloudSite and go to the config tab
	![config-tab]
4. scroll down until you reach the app settings section
5. For PHP extensions, create a PHP_EXTENSIONS key
6. For Zend extensions, create a PHP_ZENDEXTENSIONS key
	![php-zend-extensions]
7. For the value type in the location of the DLL you uploaded in step one (example below)

> If you wish to load multiple extensions or Zend extensions, create a comma separated value for the app settings **Make sure to not leave any spaces in the comma separated paths**

[Login-Link]:https://my.gearhost.com/Account/Login
[config-tab]: https://raw.githubusercontent.com/GearHost/docs/master/Images/tab-config.png
[php-zend-extensions]: https://raw.githubusercontent.com/GearHost/docs/master/Images/php-zend-extensions.PNG