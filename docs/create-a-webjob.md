# Run Background Tasks with WebJobs
You can run programs or scripts in WebJobs in your CloudSite web app in three ways: On Demand, Scheduled, or Continuous. There is no additional cost to use WebJobs.

### Acceptable file types for scripts or programs
The following file types are accepted:

- .cmd, .bat, .exe (using windows cmd)
- .ps1 (using powershell)
- .sh (using bash)
- .php (using php)
- .py (using python)
- .js (using node)
- .jar (using java)

### Create a WebJob for your CloudSite
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. **Click** the CloudSite you want to create a WebJob for
3. Click the **WebJobs tab**
4. Click **Create WebJob**

![](https://raw.githubusercontent.com/GearHost/docs/master/Images/CreateWebJob.PNG)

5. Under WebJob Name provide a name for the WebJob (the name must start with a letter or a number and cannot contain any special characters other than "-" and "_")
6. In the Select file box, click the text area and browse to the zip file that contains your script (the zip file should contain your executable as well as any supporting files needed to run the program or script)
7. Select the interval you wish to run your WebJob; On Demand, Scheduled or Continuous
8. Click Create WebJob

> For Continuous WebJobs to run, [Always On](https://www.gearhost.com/documentation/always-on) must be enabled and thus the CloudSite must be on a Small web worker node.

