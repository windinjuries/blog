---
title: nfs tutorial
date: 2023-2-25 8:00:00
tags: ssh
categories: 
- [Tutorial]
excerpt: "SSH 是 Linux 系统的登录工具，现在广泛用于服务器登录和各种加密通信"
comment: true
---


## ssh
```bash
ssh user_name@ip
```
connect to ip by openssh

## ssh-keygen
```bash
ssh-keygen -t rsa
```
generate authentication key

## ssh-copy-id
```bash
ssh-copy-id username@local_dev_board_ip
```
copy password to board linux `~/.ssh/authorized_keys`

## sftp
```bash
sftp user_name@ip

```
## scp

```bash
scp -r dir user@ip:dir
scp file user@ip:file
```
copy file by ssh
## rsync

```bash
rsync -av dir dir
```
sync file by ssh