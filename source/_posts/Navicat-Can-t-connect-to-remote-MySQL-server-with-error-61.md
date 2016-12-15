---
title: Navicat Can't connect to remote MySQL server with error 61
date: 2016-12-13 15:46:55
tags: Navicat
categories: apache
---
# Navicat无法连接远程数据库问题

标签： apache Navicat

---

## 1、Check if your mysql server is listening on a socket with netstat：
> * netstat -tulpen

![截图1](http://oaz1tuqnw.bkt.clouddn.com/eventFileList/60c98243-c21e-4f81-b2e7-d6ec9751e349.png!thumbnail)


## 2、修改/etc/mysql/mysql.conf.d/mysqld.cnf中

![截图2](http://oaz1tuqnw.bkt.clouddn.com/eventFileList/42a7779e-0b91-4c1d-a18b-b77569a2f455.png!thumbnail)

## 3、数据库重启：
> * sudo /etc/init.d/mysql restart
