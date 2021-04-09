---
title: 网络daily
date: 2021-01-04
updated: 2020-01-05
tags:
  - 学习
# password: chenyuan
# message: 这篇文章写给 Xiao.C ，请问你知道Ta是谁吗？
# categories:
# keywords:
# description: 瀚可的悄悄话，需要密码才能访问。
# top_img:
# comments:
# cover: https://s3.ax1x.com/2020/12/22/rDki5t.jpg
# toc:
# toc_number:
# copyright:
# copyright_author:
# copyright_author_href:
# copyright_url:
# copyright_info:
katex: false
# aplayer:
# highlight_shrink:
# aside:
published: false
---

# 网络daily

## 2021年1月4日

### 通信原理

在一开始，邓工以一个简化传送信息的原理图示为我们勾勒出了数据通信的大体轮廓。

![image-20210104203607497](C:\Users\hankz\AppData\Roaming\Typora\typora-user-images\image-20210104203607497.png)

由此介绍了如 

- Ethernet、Ethernet帧
- 交换机、IP地址等的简要概述

又以这样的形式介绍了数据为什么要打包、怎样打包。

![image-20210104210100722](C:\Users\hankz\AppData\Roaming\Typora\typora-user-images\image-20210104210100722.png)

说到在传输前后，数据报在各个层之间的封装与解封装，邓工就以在什么楼穿什么衣服形象地解释了这个过程。

### 实验

最后，通过一个实验，在邓工指导下学习了三层交换机来实现部分路由器的功能。虽然在过程中有着这样那样的各种小问题，但最终仍然较好地完成了“三层交换组网”实验。

过程中的命令真的很多，但在理解这些命令之后，其实会发现，每一个命令都是对应现实中一种操作。和用手机、电脑别无二致。

## 2021年1月5日

今天着重介绍了网络安全方面相关内容，有

- 静态网站的概念。
- 何为动态网站。
- 为什么要伪装成静态网站。
- 如何获悉此网站是否可注入`SQL`.
- 通过服务器连接，实验网络安全的示例。

在实验过程中，我们首先需要学会如何在服务端部署服务。进而学会如何通过主机，访问到虚拟机中的服务器。在完成这些操作之后，我们首先试探了此网站是否进行了`SQL`防注入，在一步一步利用`SQL`命令检查是否存在`账号密码表`。之后介绍了

1. ASCII猜测
2. 直接查表

这两种方法。

总的来说，今天的实训内容充实而有趣。让我们在使用SQL的同时能够了解其在网络安全方面的不足，加深了对网络安全的认识和理解。