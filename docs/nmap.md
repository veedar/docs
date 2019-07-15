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
-n - don't perform reverse DNS lookup if an active host is found
```


