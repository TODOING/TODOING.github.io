---
title: Linux常用命令
date: 2017-12-03 22:09:14
tags: Linux常用命令
categories: Linux
toc: true
---

![](/images/Linux命令.png)
<!-- more -->

## 文件和目录管理
### mkdir命令

创建目录

`语法`
> mkdir (选项)(参数)

`选项`
> -Z : 设置安全上下文，当使用SELinux时有效;
> **-m<目标属性>** 或 --mode<目标属性> : 建立目录的同时设置目录的权限;
> **-p** 或 --parents : 若所要建立的目录的上层目录尚未建立，则会一并建立上层目录;
> --version : 显示版本信息。

`参数`
> 目录 : 指定要创建的目录列表，多个目录之间用空格隔开。

`实例`
在目录`/home/pl`下建立子目录test，并且只有文件主有读、写和执行权限，其他人无权访问
> mkdir -m 700 /home/pl/test

在当前目录中建立bin下的os_1目录，权限设置为文件主可读、写和执行，同组用户可读和执行，其他用户无权访问
> mkdir -p-m 750 bin/os_1



