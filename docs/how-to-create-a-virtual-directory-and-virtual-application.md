# How to Create a Virtual Directory & Virtual Application

### Virtual Application vs Virtual Directory

The Virtual Application has it's own Session state and Application state. It is a standalone application inside the root application. 

The Virtual Directory points the physical location to a different virtual location you specify. 

### Before Getting Started
Our enviornment requires that the physical path exist on the server. Before changing or adding Virtual Directories make sure the physical path exists first. As an example if you want to change the root location from site\wwwroot to site\wwwroot\newdirectory then site\wwwroot\newdirectory should exist.

### Creating a Virtual Directory
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Click on the CloudSite you want to add the virtual directory to
1.  Toward the top click the **Config** tab
2.  Scroll until you see **Virtual Directories**
5. Click **New Virtual Directory**
6. Fill out Virtual Path and Physical Path
7. Scroll and click **Save Configuration**

### Creating a Virtual Application

1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Click on the CloudSite you want to add the virtual directory to
3. Toward the top click the **Config** tab
4. Scroll until you see **Virtual Directories**
5. Click **New Virtual Directory**
6. Fill out Virtual Path and Physical Path and make sure **Is application** is checked
7. Scroll and click **Save Configuration**

