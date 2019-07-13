---
layout: default
title: Other Tools
nav_order: 10
---


# Other Tools
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}


### convert

`convert xc:black 1x1 pixel.png` - creates an image of a single black pixel

### scp

`scp <local file> <user>@<x.x.x.x>:/x/y/z`

### SOCKS Proxy with ssh tunnel

`ssh -N -D <high port to forward i.e. 64000> <user>@<remote ip> -vvv`
 
### Geo IP Lookup

`apt install geoip-bin`  
`geoiplookup <ip address>` - shows country where the IP resides  
NOTE: DBs also be updated to show more specific info such as coordinates or cities.
