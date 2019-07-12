---
layout: default
title: Kali OS
nav_order: 2
---

# Kali OS


## System
---
`grep <string> * ` - searches for given string in all files contained in current dir  
`grep -R <string> *` - same as above but recuresively  
`grep <string> -i` - case insensitive   



`CTRL+R - reverse search` - type part of the previous command, enter when ready to execute

`locate <string> -i` - case insensitive

`chmod -x <file>` - change to executable

`/etc/rsyslog.conf` - logging configuration



## Services
---

Prcess starting/stopping etc
```
systemctl status <process>
systemclt [status|start|stop|restart] <process>
```

**View Processes**

`ps auxw | grep httpd`


## Users
---

```
adduser bob
usermod -aG sudo bob
passwd bob
su bob
```

`visudo` - edits the file of superusers 
`deluser --remove-home` bob 
`/etc/group` - shows all groups in the system 


## Packages
---

### Management
`apt update` - updates metadata in the local database    
`apt upgrade` - updates all packages in the system      
`apt upgrade <package>` - only updates that package   
`apt remove <package>`   
`apt autoremove` - removed packages that are no longer needed   
`apt-cache search <package>`    

`dpkg --list` - lists packages installed 
`dpkg -i <package>.deb` - install package 
`dpkg -c <package>.deb` - see the contents of the package 
```
apt-get
apt-cache search mlocate
apt-get install mlocate
apt-get upgrade
apt-get remove <package>
updatedb```

### Useful

 `htop`  - better version of top 
 `ufw` - uncomplicated firewall 


