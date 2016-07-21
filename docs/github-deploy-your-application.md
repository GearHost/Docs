#Continuous deployment with GitHub

Deploying files from GitHub requires that you have published your local project to GitHub repository. If you are new to GitHub this articles will help you with quick start:
* [Setup Git][setup-git]
* [Create a repository][create-a-repo]
* [Fork a repository][fork-a-repo]
* [Be social][be-social]

##Steps to setup continuous deployments in Octane with GitHub
1. Put your web application files into repository that will be used in continuous deployment. 
2. [Login to Octane][login-octane] and navigate to Publish tab under your CloudSite details page.
3. Under Continuous Deployment section click on GitHub button.
4. In the popup click Authorize to connect to GitHub.
5. New window will be opened and GitHub will ask you to login and grant permissions to Octane access to your private and public repositories.
6. Once permissions are granted Octane will ask you to pick repository and branch from which deployments will be processed.
7. To finish configruation click Activate button.
8. Your page will reload and your latest deployment will appear at the bottom.
10. To verify that web app is active click "Launch CloudSite" button. The browser should navigate you to the web app.
11. On each next push to your GitHub repo Octane will automatically build and publish new version of the web app.
12. There is a way for you to return to previous versions. Just select any inactive deployment and click "Deploy" button

##GitHub continuous deployments deactivation
1. [Login to Octane][login-octane] and navigate to Publish tab under your CloudSite details page.
2. Click "Reset Password" button at top right corner.
3. Your publishing password will be reset and GitHub deployments will be deactivated.

[setup-git]: https://help.github.com/articles/set-up-git/
[create-a-repo]: https://help.github.com/articles/create-a-repo/
[fork-a-repo]: https://help.github.com/articles/fork-a-repo/
[be-social]: https://help.github.com/articles/be-social/
[login-octane]: https://my.gearhost.com