# Database Backups

CloudPanel creates a dump of each database every night at 3:15 AM with a retention period of 7 days.

All database backups can be found in the backups directory of the site user.

```/home/$site-user/backups/```

If you have smaller databases, you can change the cron job to run more frequently, like twice a day.

To change the schedule of the database backup task, do the following:

 1. Login via SSH to your instance and become root.

```sudo su root```

 2. Open the crontab:

```nano /etc/cron.d/clp```

 3. Change the backup task schedule to your needs.

```15 3 * * * clp /usr/bin/bash -c "/usr/bin/clpctl db:backup --ignoreDatabases='db1,db2' --retentionPeriod=7" &> /dev/null```

**RETENTION PERIOD**
If you want to save the database backups for more than seven days, change the retentionPeriod value.