# How To Edit Your File/Folder Permissions
Kudu is a web interface tool to help you debug and install extensions on your CloudSite. It offers debugging tools, PowerShell access, an add-on installer, and access many other useful features! As an example, we'll use Kudu to access PowerShell and delete a directory. Before we get started you will need to retrieve your publishing credentials:

1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Select the **CloudSite** you want to edit
3. **Click** on the `publish tab` 

>**Note**: Currently you only get one username but if your password ever gets compromised you can reset it by clicking the blue button that says **"Reset Password"**

Once you have your publishing credentials:

1. Navigate to `https://{yoursitename}.scm.gear.host`. You will also need to enter your deployment credentials when prompted. Login using **$yoursitename** as the username and use your publishing password.
2. Access PowerShell by going to the **Debug Console** menu and selecting **Powershell.**
3. In this step, I'm using the **cd** command to change my working directory to /home/site/wwwroot/.  From here I can see all of my files and folders. I'll be running a command to recursively delete a folder named *setup*.

>**Tip:** You can execute scripts, or run other commands using Powershell. If you're unfamiliar with the command line you can click [here](https://blogs.technet.microsoft.com/heyscriptingguy/2015/06/11/table-of-basic-powershell-commands/) to view more detailed information. Running a Node.js application? You can check out our documentation [here](https://www.gearhost.com/documentation/getting-started-with-nodejs) for some quick tips!