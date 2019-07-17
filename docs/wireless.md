---
layout: default
title: Wireless 
has_children: true
nav_order: 5
---

# Wireless
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

### Scanning
```
airmon-ng start <wlan if> - enable monitor mode
airodump-ng <wlan if mon> - scans for wireless networks
airodump-ng -c <channel no> --bssid <BSSID> -w <file> <wlan if mon>
```
