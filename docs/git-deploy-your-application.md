# Deploy Your Application Using Git Local
Deploy your application using a **local Git** repository or online Git repositories like [GitHub](http://www.github.com) and [BitBucket](http://www.bitbucket.com) if you are using a cloud based deployment solution.

> Continuous deployments are supported.

### Installing and Configuring Local Git
1. [Visit the download site](http://git-scm.com/download/)
2. Select your **Operating System** (Windows, Mac, Linux, etc.)
3. Go through the **installation process**

### Initialize a Git Repository For Your Application
1. Open the **Terminal**, **Shell**, **Command Prompt**, or **Console** of your choice

Change to the **root directory** for your application by typing this:
```
cd {path to your root directory}
```

>**For example**: C:\Users\Username\Application1\root

Then create an empty Git repository or reinitialize an existing one:
```
git init
```
>For more syntax options [Click Here](http://git-scm.com/docs/git-init)

```
git add .
git commit -m "initial commit"
git remote add websites https://cloudsitename.scm.gear.host/cloudsitename.git
git push websites master
```

>The term *cloudsitename* is the name of your CloudSite.

Your username will be $*cloudsitename* and then your publishing password. This information can be viewed from the CloudSite Publish tab.