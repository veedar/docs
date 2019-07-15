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



