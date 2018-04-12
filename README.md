# Usage:

To take a backup of a wordpress website along with the dtabase and to store the backup in a remote server.

# Feature:

Fetchs database details automatically
Compresses the backup and uploads it to remote server

# Configuration:

* SFTP_HOST = '54.167.2.205'       

* SFTP_USER = 'backupuser'

* SFTP_KEY = '/home/ec2-user/.ssh/id_rsa' (why key over password)

* SFTP_DIR = '/home/backupuser/'

* SFTP_PORT = '22'

# Requirements:

1) Path of the directory in which the wordpress is installed 
2) Python 3.4 or above versions with the module support pysftp, sys, os, re.
3) Login credentials to the destination server in which the backup needs to be stored.

# How to run the script:

```
[root@web_server]# backup.py  /path_to_wordpress_installation
```
