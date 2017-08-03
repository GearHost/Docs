# How To Setup BitBucket
Bitbucket makes it easy for you to collaborate.  It also Provides Git and Mercurial code management for professional teams with unlimited private repositories. This guide gives steps on how to setup BitBucket on your CloudSite.

### Create a BitBucket Account
1. [Create your account](https://bitbucket.org/account/signup/) with **BitBucket**
2. Create a new **Repository**
	1. **Name** your repository
	2. Decide whether you want it **private** or not
	3. Choice what **type** of repository you want
	4. Click **Advanced Settings** if needed
3. After you have customized your repository click **Create Repository**

### Connect BitBucket with GearHost
1. Now [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. Select the **CloudSite** you wish to connect with
3. Click on **Publish** tab 
4. Select **BitBucket** under `Continuous Deployment`
5. Click **Authorize**
6. Choice your **Repository** and **Branch**
7. Click **Activate**

>**Note**: You will need to also change your Virtual Directories to:

CloudSite >> Config tab

1. Virtual Path: **/**
2. Physical Path: **site\repository**

### Clone Your BitBucket with SourceTree
1. [Download SourceTree](https://www.sourcetreeapp.com/)
2. Within the application click **Clone**
	1. Fill in the **Source Path / URL:**
	2. Fill in the **Destination Path:**
	3. Fill in the **Name:**
3. Click **Clone**

Now that you have done these steps please proceed to learn how to create a file and push it onto your website with [SourceTree](https://confluence.atlassian.com/bitbucket/copy-your-repository-and-add-files-729980492.html).

