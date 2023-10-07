## Basic Commands

| Name                     | Commands           |
| ------------------------ | ------------------ |
| Print to Screen          | `echo Hi`          |
| List files and folders   | `ls`               |
| Change Directory         | `cd my_directory`  |
| Present Working Directory| `pwd`              |


## Directories Commands

| Name                           | Commands                                           |
| ------------------------------ | -------------------------------------------------- |
| Make Directory                 | `mkdir new_directory`                              |
| Multiple Commands              | `cd new_directory; mkdir www; pwd`                 |
| Make Directory Hierarchy       | `mkdir /tmp/asia` <br/> `mkdir -p /tmp/asia/india` |
| Remove Directory               | `rm -r my_dir`                                     |
| Copy Directory                 | `cp -r my_dir /tmp`                                |
| Make Directory                 | `mkdir <directory_name>`                           |


## Files Commands
| Name                        | Commands                                                                                   |
| --------------------------- | ------------------------------------------------------------------------------------------ |
| Create new file             | `touch new_file.txt`                                                                       |
| Add Content to file         | `cat > file.txt`  <br/><br/> 1. _Add data_  <br/> 2. _Press_  `ctrl+D`                 | 
| View Content of file        | `cat file.txt`                                                                             |
| Copy file                   | `cp newfile.text copyfile.txt` <br/> `cp -v /home/thor/asia/bangalore.txt /home/thor/asia/india/bangalore` <br/> -v flag display the progress of the copy operation.                  |
| Move (Rename) file          | `mv file.txt renamefile.txt`                                                               |
| Delete file                 | `rm file.txt`                                                                              |




## Vi Editor Commands

|Name              |Commands                                                                                           |
| -----------------| --------------------------------------------------------------------------------------------------|
| Find ```Hello``` | # <ins>**Step 1**</ins>:- _Press ESC_ <br/> # <ins>**Step 2**</ins>:- Then Type <br/>```/Hello``` |



## Check OS Version

|Name              |Commands                                                                          |
| -----------------| ---------------------------------------------------------------------------------|
| Check OS Version |```ls /etc/*release*``` <br/>```cat /etc/*release*``` <br/>```cat /etc/release``` |


## Download File

|Name           |Commands                                                         |
| --------------| ----------------------------------------------------------------|
| Download File |```curl url -O <give_name>``` <br/>```wget url -O <give_name>``` |

## User Account
| Name                                                                  | Commands                       |
| --------------------------------------------------------------------- | ------------------------------- |
| User Account                                                          | `sudo ls /root`                 |
| Currently logged-in user                                              | `whoami`                        |
| Display user and group information for the currently logged-in user   | `id`                            |
| User Account                                                          | `sudo ls /root`                 |


## Services
| Name                                    | Commands                                     |
| --------------------------------------- | -------------------------------------------- |
| Start HTTPD service                     | `service httpd start`                        |
| Start HTTPD service (systemd)           | `systemctl start httpd`                      |
| Stop HTTPD service (systemd)            | `systemctl stop httpd`                       |
| Check HTTPD service status (systemd)    | `systemctl status httpd`                     |
| Configure HTTPD to start at startup     | `systemctl enable httpd`                     |
| Configure HTTPD to not start at startup | `systemctl disable httpd`                    |


## RPM Package Manager
| Name                                                                      | Commands                                     |
| ------------------------------------------------------------------------- | -------------------------------------------- |
| List all installed packages on a Red Hat-based system                     | `rpm -qa`                                    |
| Check if specific packages are installed                                  | `rpm -q ansible`                             |
| Install Package                                                           | `rpm -i ftp.rpm`                             |
| Uninstall Package                                                         | `rpm -e ftp.rpm`                             |
| Check if specific packages are installed                                  | `rpm -q ansible`                             |




sudo usermod -aG docker ubuntu







