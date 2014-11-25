---
layout:     post
title:      "Ubuntu ssh 无密码登陆"
subtitle:   "ssh-keygen, ssh-copy-id 远程登陆"
date:       2014-11-24 12:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---

<h2>1. 生成本机公私钥</h2>

`$ssh-keygen -t rsa`

<h2>2. 拷贝公钥至远程主机</h2>

`ssh-copy-id -i ~/.ssh/id_rsa.pub user@host`
<p>
	把公钥追加到服务器的.ssh/authorized_key上。
	如本机不支持ssh-copy-id命令，可手动添加。
</p>
	

<h2>3. 无密码登陆远程主机</h2>