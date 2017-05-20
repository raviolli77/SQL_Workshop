# Downloading MySQL Server for Macs

1. Download MySQL Server
2. Receive Temporary password (Save it somewhere where you won't lose it!)
3. Start MySQL Server from System Preferences
4. Run MySQL from terminal 
	
	cd /usr/local/mysql
	

5. Run 

	bin/mysql -u root -p

6. Input temp password

	tempPassword

7. Inside MySQL terminal run

	SET PASSWORD FOR 'root'@'localhost' = PASSWORD('MyNewPass');

8. Now you can access MySQL Workbench using this password 

9. To set the enviroment variable 

	vi ~/.bash_profile

10. Set the path

	export PATH=/usr/local/mysql/bin:$PATH 

11. Source yo shit 

	source ~/.bash_profile

12. Run to see if it worked

	mysql -u root -p 

If output is:

	mysql>

Success

You can now access the MySQL Server through the Workbench
