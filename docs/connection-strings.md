#Connection strings
Here we provide some examples that have worked for most applications. If you run into an issue double check your syntax in web.config. You can also search for examples online and confirm which one best works for your application. To get your database credentials login to your [portal](https://my.gearhost.com/Databases) and click on the database. Your server, database name, username and password will be provided there.


---------
####ASP Classic

**MySQL**

    connectstring = "DRIVER={MySQL ODBC 5.3 ANSI Driver};SERVER=myDBServer;DATABASE=myDatabase;UID=myUsername;PWD=myPassword;"

**MSSQL**


    "Driver={SQL Server Native Client 10.0};Server=myDBServer;Database=myDatabase;Uid=myUsername;Pwd=myPassword;"

---------
####ASP.NET
**MSSQL**

    <connectionStrings>
    <add name="SiteSqlServer" connectionString="Data Source=mssql#.gear.host;Initial Catalog=DBName;User ID=DBName;Password=Str0ngP2$$W0rd!" providerName="System.Data.SqlClient" />
      </connectionStrings>