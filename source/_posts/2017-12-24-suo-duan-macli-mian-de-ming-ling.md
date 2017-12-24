---
layout: post
title: "缩短Mac里面的命令"
date: 2017-12-24 13:51:20 +0900
comments: true
categories: 
---

首先移动到自己的Home Directory
用文本编辑器打开 .bashrc

进行alias定义，
```
alias py3='python3'
```
·bashrc文件保存

然后编辑相同目录下的 .bash_profile文件
让编辑后的 .bashrc文件生效

```
source ~/.bashrc
```

编辑完后，文件保存。

然后在Ternimal里面执行以下命令
使之编辑后的文件生效
```
source .bash_profile
```
Mac的Terminal启动的时候，先是读取 ~/.bash_profile 和 /etc/profile
然后让.bash_profile每回在被启动的时候读区里面在.bashrc文件
