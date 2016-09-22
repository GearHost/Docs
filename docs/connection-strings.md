#Connection strings
In this guide we provide the most common connection strings for applications that you can configure in your **web.config** file. You will need your database information for this to work. Please login [here](https://my.gearhost.com/Databases) and click on the database you wish to connect to your application. From there your database database server, name, username and password will be provided.



####ASP Classic

**MySQL**

    connectstring = "DRIVER={MySQL ODBC 5.3 ANSI Driver};SERVER=myDBServer;DATABASE=myDatabase;UID=myUsername;PWD=myPassword;"

**MSSQL**


    "Driver={SQL Server Native Client 10.0};Server=myDBServer;Database=myDatabase;Uid=myUsername;Pwd=myPassword;"


####ASP.NET
**MSSQL**

    <connectionStrings>
    <add name="SiteSqlServer" connectionString="Data Source=mssql#.gear.host;Initial Catalog=DBName;User ID=DBName;Password=Str0ngP2$$W0rd!" providerName="System.Data.SqlClient" />
      </connectionStrings>



>**Tip:** If these connection strings aren't working, you might be using a CMS where it places a different method of connection strings in a separate configuration file. Alternatively, you can also search for other examples online! Don't have a database? You can create one by following the instructions provided [here!](https://www.gearhost.com/documentation/create-a-database)