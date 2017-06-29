## What are deployment credentials?
***
Deployment credentials are designed to be an account level deployment user that can be used for FTP, Git, WebDeploy, etc. The username and password can be used to deploy to any CloudSite associated with your account. This keeps you from needing to create a new deployment user everytime you create a new site.

## What will the credentials be?
It's easy enough to know what your credentials are going to be. They always follow the same scheme, *site\user*.

If we had 3 sites example1, example2 and example3 and set our deployment credentials username to "awesomedeveloper" then we know how to FTP into all the sites by sligning changing our username but always keeping the same password. For example:

example1\awesomedeveloper

example2\awesomedeveloper

example3\awesomedeveloper

The password we set is also going to be the same for each one! If you change your deployment credentials username it will update it for every site.

