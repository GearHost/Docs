Migrate your Sites to GearHost 
==================

###Table of Contents
1. [Introduction](#user-content-introduction)
2. [Backing Up Your Site](#user-content-prerequisites)
3. [Restoring Your Site To GearHost](#user-content-1-install-wordpress)
4. [Preview The New Site](#user-content-2-update-wordpress-config)
5. [Updating your DNS](#user-content-3-tweaking-javascript)
6. [Conclusion](#user-content-conclusion)

***

##Introduction
Moving your site to GearHost from another host is super simple with our new platform. All that's needed is a copy of your site files and databases and some good tunes.

We can help with moving most websites over to our servers. E-Mail [Support](mailto:support@gearhost.com) anytime for a quote!


##1. Backing Up Your Site

* Site Files
* Databases
* E-Mail
 
#####Site Files
Currently you site files are being held with another provider and we need to move them to the new CloudSites servers. Your previous host will have instructions for you to download these files either via FTP or a download manager from their servers to your local machine so we can upload them in the next steps.
#####Databases
If you are using a MSSQL or MySQL database this will also need to be backed up from your previous provider and could be done through SQL Server Management Studio or phpMyAdmin. Your current host may also have an option through their control panel to download these databases.
#####E-Mail
At this time GearHost does not have a tool to import your email from a previous host's servers. A work around would be to download your email via POP3 to your local machine and store it there in an archived file. If you are connected to your mail server in a mail client such as Outlook or Mac Mail, you have the option to archive your messages into a folder that is saved locally on your machine. 
***
##2. Restoring Your Site
Now that we have everything backed up to your local machine, we can begin the process of getting your site running on CloudSites.
 
* Site Files
* Databases

#####Upload Your Site Files
There are multiple ways to publish your app to GearHost's servers. Whether it is through FTP or Microsoft Visual Studio, we have ways for you to connect. We have detailed instructions for uploading your sites files in a couple of different ways and can be found at the following links [here](https://www.gearhost.com/documentation/how-to-publish-your-app-with-ftp) and [here](https://www.gearhost.com/documentation/how-to-publish-your-app-from-visual-studio-2013).  
#####Upload Your Database
After our site files have been loaded on to our servers, we will next upload a copy of our databases. The CloudSites Control Panel has a simple upload feature and instructions for restoring can be found [here](https://www.gearhost.com/documentation/how-to-restore-a-database)
***
##3. Preview The New Site
Every CloudSite is given a preview URL for you to determine if your site is ready to be published. The preview URL will display your site exactly how it is seen on our servers and how other will see your site once it is live. More information on how to preview your site can be found at the following [link](https://www.gearhost.com/documentation/test-your-site-before-switching-DNS)
***
##4. Updating your DNS
After we have our site uploaded and our preview URL is showing the correct site we need to update the nameservers of your domain to point to GearHost. You will need to contact your registrar to make this change and help on this from major registrars can be found [here](https://www.gearhost.com/documentation/changing-nameservers) along with the GearHost nameservers.
***
##Conclusion
After all these steps are completed you now have your sites hosted with us! Keep in mind, nameserver changes can take up to 72 hours with some domain registrars and may not be immediately available. 
***



