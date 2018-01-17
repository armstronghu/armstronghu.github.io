---
layout: post
title: "linux shell命令学习"
description: ""
category: 技术
tags: [linux,shell]
---

## rm
删除除文件a，b之外的文件
```
rm -rf !(a|b)
```
如果命令出错，需要增强shell命令

```
shopt -s extglob
```

## curl
post json body
```
curl -i -d '{"appid":"xxx","begin":1501516800000,"end":1501556209000}' -H "Content-Type: application/json" -X POST http://183.36.123.87:8092/anticheat/phone/history
```

## bc
linux 计算器
```
>bc
ibase=16
obase=10
```
ibase 输入进制  obase输出进制

## hexdump
16进制查看,16进制和ascii
```
hexdump -C io/statcheck.c
```

## top
## iostat
参数 -d 表示，显示设备（磁盘）使用状态；-k某些使用block为单位的列强制使用Kilobytes为单位；2表示，数据显示每隔2秒刷新一次
```
>iostat -d -k 1 10
Device:            tps    kB_read/s    kB_wrtn/s    kB_read    kB_wrtn
sda              39.29        21.14         1.44  441339807   29990031
sda1              0.00         0.00         0.00       1623        523
sda2              1.32         1.43         4.54   29834273   94827104
sda3              6.30         0.85        24.95   17816289  520725244
sda5              0.85         0.46         3.40    9543503   70970116
sda6              0.00         0.00         0.00        550        236
sda7              0.00         0.00         0.00        406          0
sda8              0.00         0.00         0.00        406          0
sda9              0.00         0.00         0.00        406          0
sda10            60.68        18.35        71.43  383002263 1490928140

Device:            tps    kB_read/s    kB_wrtn/s    kB_read    kB_wrtn
sda             327.55      5159.18       102.04       5056        100
sda1              0.00         0.00         0.00          0          0
```
## netstat
## tcpdump
## losof

