#Deploy your application using Git


Deploy your application using a local Git repository or online Git repositories like [GitHub](http://www.github.com) and [BitBucket](http://www.bitbucket.com) if you are using a cloud based deployment solution.

> Keep in mind that we support continuous deployments as well.

###Installing and Configuring Git

If you do not have Git already please [download and install it](http://git-scm.com/download/).

###Initialize a Git repository for your application

At the command prompt, change to the root directory for your app, and then type this command:

```
git init
git add .
git commit -m "initial commit"
git remote add websites https://*cloudsitename*.scm.gear.host/*cloudsitename*.git
git push websites master
```

Your username will be $*cloudsitename* and then your password. This information can be viewed from the CloudSite Publish tab.