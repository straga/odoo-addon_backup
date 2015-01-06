odoo-addon_backup
=================

Automatic Odoo BackUP

BackUP Manager

modules list:
	backup_manager
		Main manager for backup Odoo DataBase over RPC dump.
		After installed module need change Daily BackUP and BackUP Daily Housekeeping - date time.
		(Settings->Technical->Automation->Scheduled Actions).	
		Also need determinate Directory Back path you can test it for correct path and automatically create catalog with right access.
		Add Database Server with (host, port, global password from config file)
		You can Backup any database from any servers in one place.
		You can select for each backup action, how many days backup save.
		
		Restore procedure from standard Odoo web DataBase Manager.

		
	yandex_disk
		disk.yandex.com Cloud disk storage connector to Odoo.
		Just need login and password. You can add one or more yadisk to Odoo.
		Test connection and shows available space.
Used library https://github.com/TyVik/YaDiskClient


 
	yadisk_backup_connector
		yadisk connect to BackUp Manager over yandex_disk.
		It add option to Action BackUp Manager allow upload back file to Yandex Disk.
		You can add one and more yandex disk for each backup action.
		You can select for each backup action, how many days backup save on yandex.
		Determinate directory name where on yandex disk it save.



		
	warning_popup
		Allows show warning, info, error – Message PopUp windows without exception.

extra:
	scheduler_error_mailer
  		 'name': 'Scheduler Error Mailer',
   		 'summary': 'Send an e-mail when a scheduler fails',
