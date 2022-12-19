# Importing a Database

For importing a database, CloudPanel uses mysql command-line client.

To import a database, do the following.

 1. Login via SSH with the Site User.

```ssh site-user@instance-ip-address```
 
 2. Run clpctl to see all available commands.

```clpctl```

![](https://www.cloudpanel.io/docs/v2/img/frontend-area/databases/clpctl-user-commands.png)

 3. Go to the database dump's directory and use the following command to import a database.

```clpctl db:import --databaseName=my-database --file=dump.sql.gz```