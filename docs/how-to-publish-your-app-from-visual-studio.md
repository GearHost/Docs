# How To Publish Your App From Visual Studio
Publishing your application from Visual Studio is simple and easy with GearHost regardless of your Visual Studio version.

### Download the publishing file
We make it easy to publish from Visual Studio by providing you a fully encapsulated publishing file that you will import into Visual Studio. To get this file you will need to:

1. [Log in to your GearHost account](https://my.gearhost.com/account/login)
2. Click the CloudSite name you want to upload your application to
3. Click the **Publish** tab
4. Click the Visual Studio button under the publish tab

This will download a `{cloudsitename}.{username}.publishsettings` file to your local computer storage.

### Publishing
1. **Launch Visual Studio** and open your existing web application project
2. In Solution Explorer right click on your web application and select  **Publish**
3. In the Publish wizard window at the bottom left select **Import Profile**
4. Browse to the ``{cloudsitename}.{username}.publishsettings` file you downloaded above and select **`OK`**
5. Click the **Publish button**
