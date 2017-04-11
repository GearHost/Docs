# Deploy your application using Git


Deploy your application using a local Git repository or online Git repositories like [GitHub](http://www.github.com) and [BitBucket](http://www.bitbucket.com) if you are using a cloud based deployment solution.

> Continuous deployments are supported.

#  Installing and Configuring Git

If you do not have Git already please [download and install it](http://git-scm.com/download/).

#  Initialize a Git repository for your application

At the command prompt, change to the root directory for your app, and then type this command:

```
git init
git add .
git commit -m "initial commit"
git remote add websites https://cloudsitename.scm.gear.host/cloudsitename.git
git push websites master
```

>The term *cloudsitename* is the name of your CloudSite.

Your username will be $*cloudsitename* and then your publishing password. This information can be viewed from the CloudSite Publish tab.