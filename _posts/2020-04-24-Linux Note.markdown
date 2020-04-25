---
layout:     post
title:      "Linux Note"
subtitle:   "common command"
date:       2020-04-25 22:00:00
author:     "luojiecn"
header-img: "img/post-think-try-write.jpg"
tags:
    - linux
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
