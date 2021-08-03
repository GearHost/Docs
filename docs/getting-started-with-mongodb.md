# Getting started with MongoDB
MongoDB is a [NoSQL](https://www.mongodb.com/nosql-explained) database that's scalable and optimized for big data applications. Companies such as Intuit, eBay, CitiGroup and Facebook are already using Mongo for some of their applications. While many developers have been eager to get started on Mongo, we've decided to launch this beta test so you can get started! Best of all, we're going to include **Free** and **Hobby** database plans for this as well.

### Creating a MongoDB
1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
1. Select the `Databases` menu on your left hand side 
1. Click on `Create Database` button on the top right
1. Select the plan for MongoDB

### Locate your database login credentials
1. Select the `Databases` menu on your left hand side
2. Click on your Mongo database
3. Retrieve your database login credentials

 >**Please note:** The database port is `27002`.

### Recommended MongoDB clients
For GUI clients we recommend using [MongoChef](http://3t.io/mongochef/download/) and [RoboMongo](https://robomongo.org/download).

### Connecting to your MongoDB using RoboMongo
1. Launch RoboMongo
1. Select **Create** inside the "MongoDB Connections" window prompt
1. Give your connection a name on the `Name` field
1. On the **Address** field put `den1.mongo1.gear.host` and specify your port number
1. Select the **Authentication** tab and enable the *Perform authentication* box
1. Fill out your database login credentials
1. Set **Auth Mechanism** option to `SCRAM-SHA-1`
1. Click **Test** to test your connection
1. If the test is successful, select **Save**
1. Connect to your saved connection

### Connecting using Mongo Shell
If you rather work through the command line, you can install [Mongo Shell](https://docs.mongodb.com/getting-started/shell/installation/). Fortunately, Mongo Shell is compatible with most operating systems and they provide many methods of connecting [here.](https://docs.mongodb.com/manual/reference/program/mongo/#use) If you've installed Mongo Shell on a Windows environment the following command should work for you. Please note that this is on version 3.4, so yours might slightly be different.

`<pathtomongo>bin\mongo.exe den1.mongo1.gear.host:27002/yourdb -u yourdbuser -p youruserpassword`

>**Tip:** MongoDB is case sensitive. Please be sure to always use lowercase database name and username when attempting to connect.