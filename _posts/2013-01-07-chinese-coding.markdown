---
layout: post
title: "Octopress 中文编码问题"
date: 2013-01-07 22:03
comments: true
tags:
    - tech
categories: Octopress
---
费了好大劲儿在win7系统下用Octopress搭建好博客（[鸣谢](http://chenzhiwei.net/2012/07/07/this-is-the-first-article/)），欢欢喜喜写了po，中文竟然是乱码。试了修改环境变量：

>LC\_ALL=zh_CN.UTF-8

>LANG=zh_CN.UTF-8

不成功，问google，把[帖子](http://ruby-taiwan.org/topics/46)中的方法试了一遍均不奏效（值得试一下，有成功案例）。

继续找，直到翻出v2ex上的[一帖](http://www.v2ex.com/t/26027)，回复中有人提到：

>1，markdown文件如果出现了中文请另存为UTF-8格式且去掉BOM头。

>2, yaml的冒号后要有空格。

>3, 把设置环境变量里的zh\_CN改成en\_US

照单设置，解决问题。

