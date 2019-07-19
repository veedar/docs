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

### Metasploit
```
/usr/share/metasploit-framework/
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
info <module> - show modules's info
jobs (-h) - shows active jobs
load <plugin> - loads plugin
loadpath <path> - loads a directory in the path
unload <plugin>
```
### Search
```
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
```
