---
title: 使用windows终端代替putty连接云服务器
tags:
  - ssh
  - 运维
abbrlink: 339090115
date: 2023-05-14 20:30:19
---

找 ssh 工具发现不少人推荐 putty，试了一下发现自己还是习惯使用 windows 终端，就琢磨着使用 windows 终端了

<!-- more -->
配置很简单
1. 打开 windows terminal
   1. 右键在终端中打开
   2. win+x -> 终端
   3. win+r -> 输入 cmd
      三种方式自选
2. 打开 windows terminal 的设置
3. 点击添加新配置文件，直接选择复制配置文件
4. 找到 ssh 的安装文件夹（windows 一般是"C:\Windows\System32\OpenSSH\"），复制 ssh. exe 的路径并添加到配置文件的命令行中，后面接 ssh 的参数即可，比如使用密钥就是在后面添加 `-i "私钥路径" 用户名@IP`
5. 改完直接保存即可，要使用就打开终端的菜单或是使用快捷键
