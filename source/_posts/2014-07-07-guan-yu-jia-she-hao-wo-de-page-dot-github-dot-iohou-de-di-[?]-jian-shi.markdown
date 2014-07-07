---
layout: post
title: "关于架设好我的page.github.io后的第一件事"
date: 2014-07-07 10:58:11 +0800
comments: true
categories: blog维护
---
首先想到的是，我写出来的内容要长期保留，不如托管在github.com上，思璐很简单！

在自己的github管理页中，再建一个空的repository，我把它命名为“My Pages Builder”.
然后用官方的github客户端，把它pull到本地，把我本地安装的octopress的生成器目录一并拖进去，递交的时候，ignore一些输出目录和文件就可！

然后，到哪里，只要安装好rake的环境，迁出这个repository就可以写作和提交自己的静态页了!