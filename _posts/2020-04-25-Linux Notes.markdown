---
layout: post
title:  "Linux Note"
date:   2020-04-25 22:00:00
categories: Linux bash
---

## 查看端口占用

```
使用 netstat 查看
# netstat -tnlp | grep :1080
ss 一般用于转储套接字统计信息
# ss -lntpd | grep :22
lsof(list open files)是一个列出系统上被进程打开的文件的相关信息。
lsof -i tcp:22
```
## Tmux命令

```
列出session
# tmux ls
进入已存在的session
# tmux a -t $session_name

```
## 查用户登入历史

```
# last 

```
## Ubuntu下怎么通过命令完成蓝牙的配对和连接
```shell
打开蓝牙管理器
# bluetoothctl
打开扫描
# scan on
搜索到设备后关闭扫描
# scan off 
# pair XX:XX:XX:XX:XX:XX:XX:XX
# connect XX:XX:XX:XX:XX:XX:XX:XX
```
参考链接 [蓝牙的配对和连接](https://blog.csdn.net/zhuyong006/article/details/89926521)

