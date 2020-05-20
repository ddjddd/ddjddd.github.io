---
layout: post
title: ADB Basic Usage for android debuging
categories: [Android]
authoor: Jinho Choi
---

### What's ADB?
adb: android debuging bridge

```shell
# Get device list by serial number
adb devices

# For specific device
adb -s {$Serial_number} {$CMD}

# Package install
adb install 
    -r
    -t

# Reboot
adb reboot
adb reboot download

# TCP
adb kill-server
adb start-server
adb remount

# File sharing
adb push
adb pull

# Shell
adb shell
    am
    pm
    dpm

# Getprop, feature
adb shell getprop
```
