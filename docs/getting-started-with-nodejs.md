#Getting started with Node.js
###Introduction

Node.js is a platform built on Chrome's JavaScript Engine (V8 Engine) for easily building fast and scalable network applications. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices.

----------

This document provides basic guidance on using Node.js with GearHost. 

1. [Change Node.js version](https://www.gearhost.com/documentation/getting-started-with-nodejs#user-content-change-version)
2. [Enable Websockets](https://www.gearhost.com/documentation/getting-started-with-nodejs#user-content-enable-websockets)
3. [Debugging Node.js using Kudu](https://www.gearhost.com/documentation/getting-started-with-nodejs#user-content-change-debug-your-application)
4. [Installing packages with Node Package Manager](https://www.gearhost.com/documentation/getting-started-with-nodejs#user-content-installing-packages-using-npm)
5. [Recommendations and tips](https://www.gearhost.com/documentation/getting-started-with-nodejs#user-content-recommendations)


##Change version
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Click on the CloudSite where you want to change Node.js version
3. Click the Config tab
4. Scroll down to App Settings
5. Under App Settings find the row named WEBSITE_NODE_DEFAULT_VERSION or add one if one is not present
6. Change the value to one of the [supported Node.js versions](https://www.gearhost.com/documentation/supported-technologies)
7. Click the Save Configuration button at the bottom
8. Your Node.js version is updated

##Enable Websockets
>This option is only available for Standard CloudSite plans or higher.

1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Click on the CloudSite where you want to enable Websockets
3. Click the Config tab
4. Over the Websockets menu enable the ON button

##Debug your application
The best thing to do would be to use the debug option using Kudu's PowerShell. [Here](https://www.gearhost.com/documentation/how-to-use-kudu) we provide some steps on accessing **Kudu**. As an example we will proceed with debugging my basic Node.js application.

1.	Access your Kudu portal, go to **Debug Console** and select **PowerShell**
2. Navigate to the root directory (/wwwroot/) and run `node --debug yourapp.js` As shown below you will see that we're missing a module named "express"
 
<img src="https://raw.githubusercontent.com/Gearhost/docs/master/Images/njsdebug.png" />

##Installing packages using NPM
Having a *package.json* file is useful as it provides the name of the modules required for your app. Using PowerShell, you can install an individual module by running `npm install packagename` . To make it easier you can simply run `npm install` and it will install all required modules that your *package.json* references. After installing the missing dependencies your Node.js application should start working.

##Recommendations
You can use a custom **web.config** file that's commonly used for an Azure environment like ours [here.](https://github.com/projectkudu/kudu/wiki/Using-a-custom-web.config-for-Node-apps) If you're using Visual Studio, please be sure to download [NodeJS tools](https://beta.visualstudio.com/node-js-vs/) as it's handy for publishing and debugging. We also recommend checking out troubleshooting guides and best practices from [Azure's help guide.](https://azure.microsoft.com/en-us/documentation/articles/app-service-web-nodejs-best-practices-and-troubleshoot-guide/)

>**Tip:** We close all ports by default and only leave ports 80 and 443 open for web server access. This will be an issue if you're trying to debug your application using a custom port via browser. We recommend to debug your application locally or use your Kudu for debugging.

