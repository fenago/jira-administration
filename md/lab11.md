Backing up the database


Jira stores its application data (such as issues, change history, or project information) in the database you connected during installation. To keep that data safe, use one of the methods described on this page to back up the database.There are two ways you can back up the contents of your database: 

Using native database backup tools RECOMMENDED
Using Jira's backup utility
For large Jira installations and regular backups in production, we strongly recommend that you use native database backup tools instead of Jira's XML backup service.

Native database backup tools offer a much more consistent and reliable means of storing (and restoring) data while Jira is active. When Jira is in use, there’s no guarantee that XML backups will be consistent as the database may be updated during the backup process. Jira doesn't report any warnings or error messages when an XML backup is generated with inconsistencies and such backups will fail during the restore process.

Use native database backup tools
Most databases come with built-in backup and restore tools. We strongly recommend these tools over the built-in Jira backup utility as they:

ensure the integrity of the database by taking the backup at a single point in time
are much faster and less resource-intensive than Jira's XML backup
integrate with existing backup strategies (for example, by allowing one backup run for all database apps)
may allow for incremental backups, saving disk space
avoid character encoding and format issues resulting from Jira's use of XML as a backup format
For more information on how to set up periodic database backups, see the documentation for your database. This typically involves a cron job or a Windows scheduled task invoking a command-line tool like mysqldump or pg_dump.

Use the built-in Jira backup utility
You can use the built-in Jira backup utility to take a one-off snapshot of your database in XML format.

To use the built-in Jira backup utility, you must have the Jira system administrator global permission.

When you install Jira and complete the run the setup wizard, an database backup service will run automatically every 12 hours by default. You can add additional backup services that run on different schedules, update existing service configurations, or disable automatic backups. Learn more about configuring automatic database backups

Before you begin
Make sure that Jira has the necessary file system permissions to write to the <jira-home>/export/backups directory, where <jira-home> is the Jira [shared] home directory.

To back up your database with the built-in utility:

In the upper-right corner of the screen, select Administration ()> System. 
In the side panel, under Import and export, select Backup system.
In the File name field, enter a name for the backup file.
Select Backup and wait until your Jira data is backed up. Jira will save your XML backup inside a zipped archive file under <jira-home>/export/backups.
When the backup is complete, you’ll see a message confirming that Jira has written the contents of the database to the file you specified.
Last modified on Mar 26, 2024