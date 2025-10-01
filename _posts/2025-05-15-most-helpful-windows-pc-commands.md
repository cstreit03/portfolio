---
layout: post
title: Most Helpful Commands for Windows Systems
date: 2025-05-15 21:05:29 -0500
description: A guide with some of the most helpful commands for Windows 10, Windows 11, and Windows Server machines.
tags: ["Technology", "Guides"]
categories: ["Tech Guides"]
---

# Most Helpful Commands for Windows Systems

This guide includes some of the most helpful commands I have used when working on Windows 10, Windows 11, and Windows Server machines.

---

# Most Helpful Commands for Windows Systems

This guide includes some of the most helpful commands I have used when working on Windows 10, Windows 11, and Windows Server machines.

## Check the battery health level

Manufacturer utilities like Dell SupportAssist can check the battery health, but only check the current output. To check the actual battery health level in terms of maximum battery capacity, run this command and view the report.

```bat
powercfg /batteryreport
```

## Find MAC address for a wireless AP

This command lets you find the MAC address of the Wi-Fi access point that your Windows computer is currently connected to.

```bat
netsh wlan show interfaces
```

## Flushing DNS and renew IP address

Flushing the DNS cache is a good first step when a computer is unable to reach a website or internal server. The three commands below will flush the DNS cache and renew the IP address.

```bat
ipconfig /release
ipconfig /renew
ipconfig /flushdns
```

## Retrieve unknown BitLocker keys

It seems like a slight security risk that you can recover the BitLocker keys simply by running a command. Still, this command is very helpful for automating the process of gathering BitLocker keys.

```bat
manage-bde -protectors C: -get
```

## Get Wi-Fi connection report

This command will generate a report of the Wi-Fi connection status and health.

```bat
netsh wlan show wlanreport
```

## Troubleshooting system performance

These commands are helpful on a computer that is slow, experiencing errors, or stuck on the Blue Screen of Death (BSOD). The set of commands checks for system file corruption, OS image corruption, and disk errors.

```bat
sfc /scannow
DISM /Online /Cleanup-Image /CheckHealth
DISM /Online /Cleanup-Image /ScanHealth
DISM /Online /Cleanup-Image /RestoreHealth
chkdsk /f /r
```

## Get a device serial number

Since most RMM systems rely on serial numbers for identification, it’s helpful to know how to get the serial number without being able to read the computer’s label. This command outputs the device serial number.

```bat
wmic bios get serialnumber
```

## Recover a lost Wi-Fi password

Find the Wi-Fi password on a device that is currently connected to it. Make sure to replace the WIFI_NETWORK placeholder with the actual wireless network name.

```bat
netsh wlan show profile name=“WIFI_NETWORK” key=clear
```

---
