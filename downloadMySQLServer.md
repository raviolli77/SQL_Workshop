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

Here you will enter the `bash_profile`, next you can scroll all the way to the bottom of the file and then click `i` this will then allow you to edit the script now copy paste the following section (again to the bottom of the script):

10. Set the path

	export PATH=/usr/local/mysql/bin:$PATH 

Once you have copy-pasted this you will exit out of the editing mode by hitting `esc` then you will enter `:wq` to write (so save changes) and quit (escape) the script and you should be returned to the terminal you were in before you entered the `vi` command. 

11. Source yo shit 

	source ~/.bash_profile

This will allow your computer to recognize the path we had set earlier (you can also exit the terminal and once you start a new terminal the changes will be made)

12. Run to see if it worked

	mysql -u root -p 

Recall to input the new password you set earlier when prompted to do so. 
If output is:

	mysql>

Success

You can now access the MySQL Server through the Workbench, using the credentials you made through the *MySQL* server. 
