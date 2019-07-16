---
layout: default
title: Nmap
parent: Reconnaissance
nav_order: 2
---



# Nmap
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


### Simple Scans
```
nmap x.x.x.x,2,3,4,5 - Scan set of IPs with different last octet  
nmap x.x.x.x-20 - Scan set of IPs within the range (from x to 20)  
nmap x.x.x.x/xx - Scan entire subnet  
```
```
nmap -iL <file> -  Scan hosts/networks from a text file  

Other Options:
--excludefile <file>
```

### Host Discovery
```
nmap -sL x.x.x.x - List Scan - simply list targets to scan
nmap -sn x.x.x.x - Ping Scan - disable port scan
nmap -PS/PA/PU/PY[portlist] x.x.x.x - TCP SYN/ACK, UDP or SCTP discovery to given ports, 
    - PA - ACK scan, since there is no open connection, host should respond with RST
nmap -PE/PP/PM x.x.x.x - ICMP echo, timestamp, and netmask request discovery probes

Other Options:
-n - don't perform reverse DNS lookup on an active host's IP
-D <decoy IP1> <decoy IP2> - decoy - sends other scans from spoofed IPs to decoy an IDS
```

### Port Discovery
```
nmap x.x.x.x -p <port ranges> - Only scan specified ports
nmap x.x.x.x -sS <port ranges> - TCP SYN scan (defaults to first 1000 ports)
nmap x.x.x.x -sT <port ranges> - TCP Connect Scan (works without root priv)
nmap x.x.x.x -sU <port ranges> - UDP Scan 
nmap x.x.x.x -sN; -sF; -sX - TCP NULL, FIN, and Xmas scans
nmap x.x.x.x -sA - TCP ACK scan
nmap x.x.x.x -sA - TCP ACK scan
nmap x.x.x.x -sO - IP protocl scan (TCP, ICMP, IGMP, etc)

Other Options:
--exclude-ports <port ranges>
```

### Service and Version Detection
```
-sV <IP> <port ranges> - Probe open ports to determine service/version info.

Other Options:
--version-intensity <level>: Set from 0 (light) to 9 (try all probes)
```

### Identifying the Operating System

```
```

### Vulnerability Scans
```
```
