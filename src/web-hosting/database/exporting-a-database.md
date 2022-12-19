# Exporting a Database

For exporting a database, CloudPanel uses mysqldump client utility.

To export a database, do the following.

 1. Login via SSH with the Site User.

```ssh site-user@instance-ip-address```

 2. Go to the directory where the database dump should be saved e.g., the tmp directory of the user.

```cd ~/tmp/```

 3. Run clpctl to see all available commands.

```clpctl```

![](https://www.cloudpanel.io/docs/v2/img/frontend-area/databases/clpctl-user-commands.png)

 4. Use the following command to export a database.

**COMPRESSION** The database dump will be gzipped if you add .sql.gz at the end of the file name. If you want to export the database uncompressed, use .sql.

```clpctl db:export --databaseName=my-database --file=dump.sql.gz```