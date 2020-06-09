---
layout: post
title: ADB Basic Usage for android debuging
categories: [Android]
authoor: Jinho Choi
---

## What's ADB?
### ADB: android debuging bridge
  
> ADB는 기기와 연결하여 다양한 명령을 수행할 수 있는 도구로써, 어플리케이션 설치나 디버깅 등의 작업을 수행 가능함.  
> 다양한 명령어 실행에 필요한 Shell 관련 명령어 제공  
> https://developer.android.com/studio/command-line/adb

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
