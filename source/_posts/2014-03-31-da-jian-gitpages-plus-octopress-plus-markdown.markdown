---
layout: post
title: "搭建gitpages+octopress+markdown"
date: 2014-03-31 22:12:50 +0800
comments: true
categories: 
---
###名词解释

gitpages: github上的个人主页，除了个人主页外还有项目主页，在每个项目的gh-pages分之上，github默认会发布该分之

octopress: 简化blog的生成，发布markdown格式文件到edwinmin.github.io项目的master上，使程序员能专注于记录

markdown: 文本标记语言，比html更简洁

<!--more-->

###环境搭建

[环境搭建详细文档](http://chensy0203.github.io/posts/hello-octopress.html)

###遇到问题

####bundle install安装错误
安装过程如果出现错误，需要重新安装ruby,且需要用rvm安装最新版本
<pre>
# 安装rvm
curl -L https://get.rvm.io | bash -s stable
source ~/.rvm/scripts/rvm
# 安装ruby最新版本
rvm install ruby --head
</pre>

####rake deploy时无法push到master分支
<pre>
直接复制edwinmin.github.io项目的.git目录到/octopress/_deploy/下覆盖更新.git文件
</pre>