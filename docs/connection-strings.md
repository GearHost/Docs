# Connection strings
A connection string connects your application to your database. In this guide we'll provide some examples you can use! You will need your database credentials for this to work. Login to  [your account](https://my.gearhost.com/Databases) and select your database. Here we provide your  **Database Server**, **Name**, **Username** and **Password**.



#### ASP Classic

**MySQL**

    connectstring = "DRIVER={MySQL ODBC 5.3 ANSI Driver};SERVER=mysql#.gear.host;DATABASE=DBName;UID=DBUser;PWD=myPassword;"

**MSSQL**


    "Driver={SQL Server Native Client 10.0};Server=mssql#.gear.host;Database=DBName;Uid=DBUser;Pwd=myPassword;"


#### ASP.NET
**MySQL**

    <connectionstrings>
      <add name="AppNameCString" connectionstring="Data Source=mysql#.gear.host;Initial Catalog=DBName;User Id=DBUser;Password=myPassword" providername="MySql.Data.MySqlClient" />
    </connectionstrings>


**MSSQL**

    <connectionStrings>
    <add name="AppNameCString" connectionString="Data Source=mssql#.gear.host;Initial Catalog=DBName;User ID=DBUser;Password=myPassword" providerName="System.Data.SqlClient" />
      </connectionStrings>



>**Tip:** If these connection strings aren't working, you might be using a CMS where it reads the connection strings from a separate file. You can also search for other examples online. Don't have a database? You can create one by following the instructions provided [here!](https://www.gearhost.com/documentation/create-a-database)