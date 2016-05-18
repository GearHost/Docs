#Debugging your ASP.NET application using web.config
----------
Below we'll walk you through setting up debugging on your application.

----------


You may be publishing an application only to later see this image below instead of your content. This error itself is not really verbose, so you will need to enable debugging on your application.
<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/debugasp1.PNG"/>

You will need to edit your **web.config** file which should be located in **/site/wwwroot/**. Below the *<system.web>* flag add `<customErrors mode="Off"/>` as shown below and publish the new changes.


<img src="https://raw.githubusercontent.com/gearhost/docs/master/Images/debugasp2.PNG"/>


Now that you've saved your changes, your website should display a more verbose error that should look something like this. Now we've determined that there is a coding error on line 4 under *Default.aspx.cs*

<img src="https://raw.githubusercontent.com/gearhost/docs/master/Images/debugasp3.PNG"/>

Enabling debugging is useful to determine the root cause when a *Server Error* shows up. You can also enable Site Diagnostics and we have a guide included [here.](https://www.gearhost.com/documentation/site-diagnostics) 

----------
**Tip:** Are you using Classic ASP and can't enable debugging? We have an article for that provided [here.](https://www.gearhost.com/documentation/enable-classic-asp-errors)You can also search for other methods to enable debugging online.