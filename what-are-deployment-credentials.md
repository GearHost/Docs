##What are deployment credentials?
***
Deployment credentials are designed to be an account level FTP user. The username and password can be used to deploy to any CloudSite associated with the account you use to log into your my.gearhost.com. This keeps you from needing to create a new FTP user everytime you create a new site.

##What will the credentials be?
It's easy enough to know what your credentials are going to be. They always follow the same scheme, site\user. 

If we had 3 sites, example1.com example2.com example3.com and set our deployment credentials to gearhost1 then we know how to FTP into all the sites. Take a look!

example1\gearhost1

example2\gearhost1

example3\gearhost1

The password we set is also going to be the same for each one! If you change your deployment credentials username it will update it for every site.

