---
layout: post
title: "第一次rake deploy失败的对策"
date: 2014-07-07 11:11:38 +0800
comments: true
categories: 
---

运行 rake deploy后出现以下消息

#### Pushing generated _deploy website
To https://github.com/CornerZhang/cornerzhang.github.io.git

 ! [rejected]        master -> master (non-fast-forward)
 
error: failed to push some refs to 'https://github.com/CornerZhang/cornerzhang.github.io.git'

hint: Updates were rejected because the tip of your current branch is behind

hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.

hint: See the 'Note about fast-forwards' in 'git push --help' for details.

#### Github Pages deploy complete


然后网上找了下，这种方式简单有效：

1 进入_deploy/目录

2 先执行git pull

3 然后再执行 git push --force origin master 

4 替换原先的git push -u origin master