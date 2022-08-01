[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate?business=QVR5JEKFBASVW&no_recurring=0&currency_code=USD)
# INCREMENTAL OR SYNC BACKUP TO UNRAID FOLDER - by bdrtec
	This script make incremental or sync backup to a folder.

	It's possible to schedule how often and what type of the backup will be done.

	When the backup start, you'll be notified by the email. When it finishes, too.

# INCREMENTAL BACKUP
	Don't delete anything from the backup directory, just copy new or modified files.
	
 	Schedule the execution frequency in "CA User Scripts -> Schedule Disabled".
	Example: "Schedule Daily" or "Schedule Weekly".

# SYNC BACKUP
	Mirroring. If the file isn't in the source directory, it'll be deleted from the backup directory.
	
	How often to backup is defined in the script.
	Example: sync backup every 30 days from the last backup.
			
# INSTRUCTIONS
	- Create a script in "CA User Scripts / Script_Name"
	  (Unraid -> Settings -> User Scripts -> Script_Name").

  	- Configure the variables in "script".

	- The folder and all files will be created in "Src_Flash / Script_Name"
	  (/boot/config/plugins/user.scripts/scripts/Script_Name")
	  and a copy in "Script_Dir / Script_Name".

	- Add the path of the folders you want to backup in "Script_Dir / Script_Name / PATHS.txt".

	- Run the "script" again to sync all files and start the backup.
