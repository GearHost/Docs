##How to connect to a MySql Database
#####Prerequisites

Create or [restore] a MySql Database
####Steps

1. Get your credentials
	
	a. Select your database tab
	
    ![dbtab][db-tab]

	b. Select the database

    ![selectdb][select-db]

	c. Select Show/Hide Password to seee your password
	
	![showhide][show-hide]
	
	d. Note your username and password under the database users, and database server under the database details
	
	![dbdetails][db-details]

2. Log in to MySQL Workbench with your credentials

	a. Select database -> connect to database
	
	![wbdb][workbench-db]

	b. Enter your Database server and username 

	![wb-creds][enter-creds]

	c. Store your password in the vault
	
	![vault]

	c. Confirm by selecting ok
	
	d. You are now connected!


[restore]: https://www.gearhost.com/documentation/how-to-restore-a-database
[db-tab]: https://raw.githubusercontent.com/GearHost/docs/master/Images/menu-databases.png
[select-db]: https://raw.githubusercontent.com/GearHost/docs/master/Images/select-db.png
[show-hide]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-showhidepassword.png
[db-details]: https://raw.githubusercontent.com/GearHost/docs/master/Images/db-server.png
[workbench-db]: https://raw.githubusercontent.com/GearHost/docs/master/Images/database-workbenchdatabase.png
[enter-creds]: https://raw.githubusercontent.com/GearHost/docs/master/Images/workbench-enter-creds.png
[vault]: https://raw.githubusercontent.com/GearHost/docs/master/Images/workbench-vault.png