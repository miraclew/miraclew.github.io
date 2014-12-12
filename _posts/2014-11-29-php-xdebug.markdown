---
layout:     post
title:      "PHP 使用 Xdebug"
subtitle:   "var_dump, remote debug"
date:       2014-11-29 14:00:00
author:     "miraclew"
header-img: "img/post-bg-06.jpg"
---

<h2>安装xdebug</h2>

`brew install php55-xdebug`

<h3>更美观的调试信息输出</h3>
当使用 var_dump, print_r 时，页面输出更美观的调试信息

在php.ini, 打开html_errors选项

<h3>配置远程调试</h3>

    zend_extension = 'php55-xdebug.so'
    xdebug.auto_trace=1

    xdebug.collect_params=1
    xdebug.collect_return=1
    xdebug.trace_output_dir="/tmp/xdebug/trace"
    xdebug.profiler_enable=1
    xdebug.profiler_output_dir="/tmp/xdebug/profiler"

    xdebug.remote_autostart = 1
    xdebug.remote_enable = 1
    xdebug.remote_host = localhost
    xdebug.remote_port = 9000
    xdebug.remote_handler=dbgp

