# SSH/FTP

## SSH

The SSH protocol (also referred to as Secure Shell) is a method for securing remote login from one computer to another.
It provides several alternative options for strong authentication, and it protects the communication's security and integrity with strong encryption.

### Add User

To add a new SSH User, click on the tab SSH/FTP and enter a User Name and Password and click on Add User.

![](https://media.discordapp.net/attachments/1052025865803939880/1053117886518009936/image.png)
![](https://media.discordapp.net/attachments/1052025865803939880/1053118265997656074/image.png)

### Deleting a User

To delete an SSH User, click on the tab SSH/FTP and then on Delete and confirm your action.

### Password Change

To change the password for an SSH User, click on the tab SSH/FTP and then on the User Name.

Enter a new strong Password or click on Generate new password and click on Save.

![](https://media.discordapp.net/attachments/1052025865803939880/1053118764255825950/image.png)

### SSH Login

To login via SSH to the instance, you need a terminal like iterm2 for macOS or putty for Windows.

The SSH port is 22 (default port). Before you try to connect with SSH, make sure that port 22 is open for your ip address.

**Linux and MacOS:**

**SSH login via password**

```ssh john-doe@instance-ip-address```

**SSH login via private key**

```ssh -i path_to_your_private_key.pem john-doe@instance-ip-address```

**Windows:**

In the Host Name field, enter the instance ip address and click on the button Open.

![](https://www.cloudpanel.io/docs/v2/img/frontend-area/ssh-ftp/putty-ssh.png)

Putty will ask you to enter the User Name and Password in the next step.

### SFTP Login

To login via SFTP to the instance, you need a client like [FileZilla](https://filezilla-project.org/).

Make sure that the SSH port 22 is open for your ip address.

Enter the Host, Username, Password and Port fields and click on the button Quickconnect.

**PORT**
Make sure to use port 22 for an SFTP connection.

![](https://www.cloudpanel.io/docs/v2/img/frontend-area/ssh-ftp/sftp-login-filezilla.png)

## FTP

The File Transfer Protocol (FTP) is a standard network protocol used to transfer computer files between a client and server on a computer network.

### Adding a User

To add a new FTP User, click on the tab SSH/FTP and enter a User Name, Password, and Home Directory and click on Add User.

![](https://media.discordapp.net/attachments/1052025865803939880/1053119754744909844/image.png)

### Deleting a User

To delete an FTP User, click on the tab SSH/FTP and then on Delete and confirm your action.

![](https://media.discordapp.net/attachments/1052025865803939880/1053119937251651664/image.png)

### Password Change

To change the password for an FTP User, click on the tab SSH/FTP and then on the User Name.

Enter a new strong Password or click on Generate new password and click on Save.

![](https://media.discordapp.net/attachments/1052025865803939880/1053120067434467338/image.png)