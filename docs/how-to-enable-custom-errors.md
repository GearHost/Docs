# How To Enable Custom Errors 
Below we'll walk you through setting up custom errors in web.config

### Example of an error
You may be publishing an application only to later see this error below instead of your content. This error itself is not really verbose, so you will need to enable custom errors.
<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/debugasp1.PNG"/>

### How to enable custom errors
You will need to edit your **web.config** file which should be located in **/site/wwwroot/**.

Below the "system.web" flag **add** `<customErrors mode="Off"/>` and **publish** the new changes. It should look something like this:
<img src="https://raw.githubusercontent.com/gearhost/docs/master/Images/debugasp2.PNG"/>

###Example of a custom error
Now that you've saved your changes, your website should display the custom error that should look something like this. Now we've determined that there is a coding error on line 4 under *Default.aspx.cs*
<img src="https://raw.githubusercontent.com/gearhost/docs/master/Images/debugasp3.PNG"/>

Enabling custom errors is recommended when you see a *Server Error* so you know where to start your troubleshooting. You can also enable Site Diagnostics and we have a guide included [here.](https://www.gearhost.com/documentation/site-diagnostics) 

>**Tip:** Are you using Classic ASP and can't enable errors? We have an article for that provided [here.](https://www.gearhost.com/documentation/enable-classic-asp-errors)