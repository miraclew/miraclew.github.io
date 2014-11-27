---
layout:     post
title:      "Linux watch命令"
subtitle:   "Linux下重复执行命令，观察结果"
date:       2014-11-27 14:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---

<h2>Watch</h2>


<h3>观察PHP进程</h3>
`watch -n 2 'ps aux|grep php'`

<p>-n: 是时间间隔</p>

<h3>观察文件系统变化</h3>
 `watch -d ls -l`