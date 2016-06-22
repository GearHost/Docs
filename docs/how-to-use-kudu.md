###How to use KUDU

----------

KUDU is a UI to help you diagnose and debug your Azure Web Site. It offers debug tools, Powershell access, modify add-ons, access many other useful features! As an example, we will give using a cloudsite called **zpma.** We'll use Kudu to access powershell to delete a directory as FTP can take longer when deleting big directories.

----------

Navigate to http://[yoursitename].scm.gear.host. You will also need to enter your deployment credentials when prompted. Login using **$yoursitename** as the username and use your publishing password for that cloudsite. Your address bar should look something like this:

<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/kudu1.PNG" />


After you enter your credentials, you will be logged into the Kudu interface. You can access Powershell by going to the **Debug Console** menu and selecting **Powershell.**


<img src="https://raw.githubusercontent.com/Gearhost/docs/master/Images/kudu3.PNG"  />


In this step, I'm using the **cd** command to change my directory to /home/site/wwwroot/.  From here I can see all of my files and folders. I'll be running a command to recursively delete an entire folder.

<img src="https://raw.githubusercontent.com/Gearhost/docs/master/Images/kudu4.PNG" />



----------
**Tip:** You can execute scripts, or run other commands using the Powershell interface. If you're unfamiliar with the command line, you can click [here](https://blogs.technet.microsoft.com/heyscriptingguy/2015/06/11/table-of-basic-powershell-commands/) to view more detailed information.