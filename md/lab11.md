## Lab: Backing up the database


Jira stores its application data (such as issues, change history, or project information) in the database. To keep that data safe, back up the contents of your database.

**Use the built-in Jira backup utility**

You can use the built-in Jira backup utility to take a one-off snapshot of your database in XML format.

When you install Jira and complete the run the setup wizard, an database backup service will run automatically every 12 hours by default. You can add additional backup services that run on different schedules, update existing service configurations, or disable automatic backups. Learn more about configuring automatic database backups

To back up your database with the built-in utility:

1. In the upper-right corner of the screen, select **Administration** > **System**. 

2. In the side panel, under **Import and export**, select **Backup system**.

3. In the **File name** field, enter a name for the backup file.

3. Select **Backup** and wait until your Jira data is backed up. Jira will save your XML backup inside a zipped archive file under `<jira-home>/export/backups`.
When the backup is complete, you’ll see a message confirming that Jira has written the contents of the database to the file you specified.
