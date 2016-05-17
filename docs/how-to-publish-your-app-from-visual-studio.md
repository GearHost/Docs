##How to publish your app from Visual Studio

----------

Below we'll walk through setting up deployment credentials and using those in Visual Studio to publish your application. If you have already done this, proceed with the next section.

----------

Login to your hosting [portal.](https://my.gearhost.com)

Click on your Cloudsite's name and select the **Publish** menu.

Click on the Visual Studio icon to download your publishing file. Now that you have your publishing file, go back to Visual Studio.

<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/vstudio.PNG"  />

##Publishing


Open **Solution Explorer** (can be enabled using the *Views* menu) and right click on the project name. Then select **Publish Web App** or if you see a **Publish ...** option that works too.
Your site cannot be running in debug mode for this option to appear. 

<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/vstudio1.PNG"  />

Click on **Import**, browse for the publishing file you previously downloaded and select OK.
<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/Vstudio2.PNG"  />


You will see that your settings are filled out and can select "Validate Connection" to ensure it's working properly. If everything is working on your end, select the **Publish** option to begin uploading your files.
<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/vstudio3.PNG"  />

----------

**Tip:** Visual Studio provides an output every time you publish files. Errors can be anything from an invalid SQL connection, to syntax errors. Try searching online for errors you may be receiving.