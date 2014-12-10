##Creating a DSN-less connection string

You do not need to use an ODBC datasource to connect to your database, in fact this is actually a slower method. Using a DSN-less connection string is a more effective method.
 
We apologize for the inconvenience this may cause some of our customers, but GearHost does not support ODBC datasources (DSN) with CloudSites. We have provided a few DSN-less connection string examples below. Remember these are only examples, and you will be required to place these in your applications. 

###ASP.NET
ASP.NET connection strings usually go in the web.config file. 

###MSSQL Server 2008

Data Source=myServerAddress;Initial Catalog=myDataBase;User Id=myUsername;Password=myPassword;

###Access Database

Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:CloudSites\6-Digit-myCloud-#\cloudsite-domain.com\data\mydatabase.mdb;

###PHP
We advise using an include file or config file to store your connect string, so it is easier to change later on. 

###MySQL
This is some simple code that will connect and error if the connection does not work. 

<?php
$link = mysq#_connect('localhost', 'mysq#_user', 'mysq#_password');
if (!$link) {
    die('Could not connect: ' . mysq#_error());
}
echo 'Connected successfully';
mysq#_close($link);
?>