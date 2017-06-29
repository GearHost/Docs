# How to publish your app from Visual Studio
Publishing your application from Visual Studio is simple and easy with GearHost regardless of your Visual Studio version.

### Download the publishing file
We make it easy to publish from Visual Studio by providing you a fully encapsulated publishing file that you will import into Visual Studio. To get this file you will need to:

1. [Log in to your GearHost account](https://my.gearhost.com/account/login)
2. Click the CloudSite name you want to upload your application to
3. Click the `Publish` tab
4. Click the Visual Studio button under the `Application Publishing Files` heading

This will download a `{cloudsitename}.publish` file to your local computer storage.

### Publishing
1. Launch Visual Studio and open your existing web application project
2. Right click on your web application and select `Publish Web App`
3. In the Publish wizard window select Profile and select `Import` under the `Select a publish target` menu
4. Browse to the `{cloudsitename}.publish` file you downloaded above and select `OK`
5. Click the Publish button

![](https://raw.githubusercontent.com/GearHost/docs/master/Images/vspublish.png)