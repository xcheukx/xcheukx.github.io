---
layout: post
title:  "去除Enter passphrase for key"
date:   2017-08-07 14:51:00 +0800
cover: "assets/img/cover/3.png"
tags: [git]
---
之前在创建ssh key时，由于设置了密码，导致每次git操作都出现Enter passphrase for key，搞得很麻烦。
下面是解决方法，复制原有的ssh key，然后修改掉密码成空就可以了。
ssh-keygen -p
回车后会提示enter the keyfile location，输入id_rsa文件的路径就可以了，回车。
然后再输入原本的密码，接着new passphrase这直接回车就解决了。