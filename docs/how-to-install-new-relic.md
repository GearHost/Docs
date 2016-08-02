##How to install New Relic Agent on your cloudsite.

Using New Relic's monitoring service is a great way to monitor your .NET application, and it's also absolutely free!
Before you start you will need your New Relic license key. 
You can retrieve it by following this [guide.](https://docs.newrelic.com/docs/accounts-partnerships/accounts/account-setup/license-key#finding)

----------


Navigate to http://[yoursitename].scm.gear.host.

Login using "$yoursitename" as the username and use your publishing password for that cloudsite.


<img src="https://raw.githubusercontent.com/Gearhost/docs/master/Images/relic1.PNG" />

From the top navigation, select **Site Extensions** and click on **Gallery.**

Next to the **New Relic** site extension, select the **+** icon to install. 

<img src="https://raw.githubusercontent.com/Gearhost/docs/master/Images/relic2.PNG" />

Allow a minute or two for the installation to complete.

After it's installed, login to your octane [portal](https://my.gearhost.com) and restart your application pool.
If you're not familiar with doing this procedure, follow this [guide.](https://www.gearhost.com/documentation/managing-your-application-pool-start-stop-or-restart)

On your cloudsite menu select **Config** and go to **App Settings**. Add the following key and values;


    COR_ENABLE_PROFILING	1
    COR_PROFILER	{71DA0A04-7777-4EC6-9643-7D28B46A8A41}
    COR_PROFILER_PATH	\site\wwwroot\newrelic\NewRelic.Profiler.dll
    NEWRELIC_HOME	\site\wwwroot\newrelic
	NEW_RELIC_LICENSE_KEY YOUR_LICENSE_KEY


It should look something like this: 

<img src="https://raw.githubusercontent.com/Gearhost/docs/master/Images/relic3.PNG" />

Connect to your cloudsite through FTP, navigate to **/site/wwwroot/newrelic** and edit your **newrelic.config** file.

On line 5 replace **"REPLACE_WITH_LICENSE_KEY"** with your license key.

On line 7 replace **"c:\Home\LogFiles\NewRelic"** with **"\LogFiles\NewRelic"**

Save the changes and restart your application.

You can view your app's recorded data by going to their website and selecting the **APM** menu. 
We recommend at least waiting 10-15 minutes for New Relic to start gathering your information.


>**Tip:** You can follow their official documentation [here.](https://docs.newrelic.com/docs/agents/net-agent/azure-installation/azure-portal)You can also download their official app on your android or apple device!
