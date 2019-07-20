---
layout: default
title: Metasploit
parent: Exploitation
nav_order: 2
---

# Metasploit
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

### Metasploit Directories
```
/usr/share/metasploit-framework/ - root
/usr/share/metasploit-framework/data/wordlists/ - wordlists
```
```
msfconsole - starts MSF
```
### Basics
```
banner - shows banner
? - help
help <option> - detailed help
color <option> - sets console colours
connect <options> - connects to a host (similar to netcat)
edit <file> - vim editing
grep <options> - search for modules
info <module/path> - show modules's info
jobs (-h) - shows active jobs
load <plugin> - loads plugin
loadpath <path> - loads a directory in the path
unload <plugin>

workspace (-h) - shows the workspaces
workspace -a <name> - creates (and switches to) new workspace
workspace -d <name> - deletes a workspace
workspace <name> - switches workspaces
```
### Search
```
help search
search <word>

Options:
  name:<word>
  type:<type>
  author:<name>
  platform:<platform>
  cve:<part of CVE e.g. year>

Types:
  payload
  
Platforms:
  linux
  windows
  
show [payloads | exploits] (grep <str>)
```

### Set
```
use <module> 
show options <of the module>
show targers - displays the targers set
show advanced - displays advanced options

set <option> <value> - setting a local variable (e.g. RHOST)
setg <option> <value> - setting a global variable (e.g. RHOST)
unset

```
### Initial Database Setup
```
systemctl start postgresql
msfdb init

msfconsole
  db_status
```

### Other
```
db_nmap <nmap options> - runs nmap and adds results to local db
hosts - lists found hosts
services - lists found services (help services)
  -c 
    name,port

help database

vulns (-i) - shows info for all services in db
vulns -p <port/port-range> -i - show vulns for services in db
```
### Exploit
```
use <exploit>
show options
set <option>
run

sessions -l - shows open sessions
sessions -i <number> - interacts with existing session
```
### Post Exploitation

Add your public ssh key to ~/.ssh/authorized_keys  
Enable RSAAuthentication in the SSH config file

