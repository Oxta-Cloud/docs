# Cron Jobs

Cron is one of the most valuable utilities that you can find in any Unix-like operating system.
It is used to schedule commands at a specific time. These scheduled commands or tasks are known as Cron Jobs.

## Adding a Cron Job

**Via CloudPanel**

To add a Cron Job, click on the Cron Jobs tab, select a Template and enter the Command you want to execute.

![](https://media.discordapp.net/attachments/1052025865803939880/1053121129071525909/image.png)

### Via Command Line

The standard linux way to configure Cron Jobs on the command line can be used as well.

 1. Login via SSH with the Site User.

```ssh site-user@instance-ip-address```
 
 2. Enter the following command to edit Cron Jobs:

```crontab -e```

 3. Configure your Cron Job.

On the following [site](https://tecadmin.net/crontab-in-linux-with-20-examples-of-cron-schedule/), you find some useful examples of how to configure them.

### Deleting a Cron Job

To delete a Cron Job, click on the Cron Jobs tab and click on Delete and confirm your action.

![](https://media.discordapp.net/attachments/1052025865803939880/1053121747018330203/image.png)

