Git Deploying Your Application
==================

###Table of Contents
1. [Introduction](#user-content-introduction)
2. [Prerequisites](#user-content-prerequisites)
3. [Installing and Configuring Git](#user-content-1-Installing-and-Configuring-Git)
4. [Initialize a Git repository for your application](#user-content-2-Initialize-a-Git-repository-for-your-application)
5. [Deploy Application to CloudSite](#user-content-3-Deploy-Application-to-cloudsite)

***

##Introduction
The content in this article covers deploying an application or website from a Git repository.  We also support online Git repositories like [GitHub][git-download] and [BitBucket][bitbucket-link] if your team is using a cloud based deployment solution.


##Prerequisites
You must have an account set up and you must have a cloudsite added to the account if you need assistance with these items you can reference the following articles:
 
* [Set Up Account][login-link]
* [Create First Cloudsite][create-cloudsite]


***
##1. Installing and Configuring Git

>You do not need to do this step if you already have Git installed on your local computer*

 
* [download Git][git-download]
* Install Git
* Setting up Git
 
###Download Git
You will need to download Git from the main download site [here][git-download]

###Install Git
Before you start using Git, you have to make it available on your computer. Even if it’s already installed, it’s probably a good idea to update to the latest version. You can either install it as a package or via another installer. 

Git is supported on many platforms and each platform will have it's own unique way to install git.

  
- [Install Git on Windows][windows-git]
- [Install Git on Mac][mac-git]
- [Install Git on Linux][linux-git]

##Setting up Git
 
- On your computer, open the Git Shell application.
- Tell Git your name so your commits will be properly labeled. Type everything after the $ here:

```
$git config --global user.name "YOUR NAME"
```

- Tell Git the email address that will be associated with your Git commits. The email you specify should be one that you can access as it will be public to all your git consumers.

```
$git config --global user.email "YOUR EMAIL ADDRESS"
```

##2. Initialize a Git repository for your application

At the command prompt, change to the root directory for your app, and then type this command:

```
git init
git add .
git commit -m "initial commit"
```

At the command prompt, change to the root directory for your app, and then type this command:

>NOTE: This link will be provided under your git tab already construsted however you need to change https:// to http:// and you will need to remove :443 from the middle of the link provided in the control panel

>You will need to replace the deploymentuser and cloudsitename in the URL below with your information

``` 
git remote add websites http://deploymentuser@cloudsitename.scm.gear.host/cloudsitename.git
git push websites master
```



[login-link]: https://my.gearhost.com/account/signup
[git-download]: http://git-scm.com/download/
[bitbucket-link]: http://bitbucket.com
[create-cloudsite]: https://www.gearhost.com/documentation/create-a-cloudsite
[linux-git]: http://git-scm.com/book/en/v2/Getting-Started-Installing-Git#Installing-on-Linux
[mac-git]: http://git-scm.com/book/en/v2/Getting-Started-Installing-Git#Installing-on-Mac
[windows-git]: http://git-scm.com/book/en/v2/Getting-Started-Installing-Git#Installing-on-Windows


 
