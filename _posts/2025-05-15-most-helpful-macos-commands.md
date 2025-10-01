---
layout: post
title: Most Helpful Commands for macOS
date: 2025-05-15 21:05:29 -0500
description: A guide with some of the most helpful commands for Apple macOS computers.
tags: ["Technology", "Guides"]
categories: ["Tech Guides"]
---
# Most Helpful Commands for macOS

This guide includes some of the most helpful commands I have used when working on Apple macOS computers. Some of them might also work on Linux though the focus here is macOS. 

## Give a user admin rights

I’ve used this mostly when the local admin account is not actually an administrator. These commands work best when the device is managed by an RMM. If you can run these commands in the background, you can give a user admin rights. 

```bash
sudo dseditgroup -o edit -a <USERNAME> -t user admin
sudo dseditgroup -o edit -a <USERNAME> -t user wheel
```

## Force a user to logout

This is helpful when you need to force users to change their password or update a MDM profile. Running one command should suffice, but sometimes only one of these work. 

```bash
sudo launchctl bootout gui/$(id -u <username>)
OR
sudo launchctl bootout user/$(id -u <username>)
```

## Change the hostname

This is more of a script than a command considering it has so many parts. Make sure to replace “COMPUTER-02” with the desired name. 

```bash
#!/bin/bash

# Change the below field 
hostname=COMPUTER-02

sudo scutil --set HostName $hostname
sudo scutil --set HostName $hostname
sudo scutil --set ComputerName $hostname
dscacheutil -flushcache
```

## Flush the DNS cache

This is helpful when troubleshooting DNS issues on the network. For example, if an employee cannot access Microsoft.com, clearing the cache could help resolve the issue. 

```bash
sudo dscacheutil -flushcache
sudo killall -HUP mDNSResponder
```
