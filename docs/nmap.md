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

Options:
--excludefile <file>
```

### Host Discovery
```
nmap -sL x.x.x.x - List Scan - simply list targets to scan
nmap -sn x.x.x.x - Ping Scan - disable port scan
nmap -PS(optional: port/port-list/port-range, no space) x.x.x.x - TCP SYN scan (defaults to firsr 1000 ports)
nmap -PA(optional: port/port-list/port-range, no space) x.x.x.x - TCP ACK scan (defaults to firsr 1000 ports), since there is no open connection, host should respond with RST

```


