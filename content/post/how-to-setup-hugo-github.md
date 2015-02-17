+++
date = "2015-02-18T00:38:59+08:00"
title = "Setup Hogo on Github How to"
author = "nehe"
tag = ["hugo", "howto"]
categories = ["howto", "Hugo"]
+++

Hugo是一个轻量级的静态网站生成系统，可以帮助你很迅速的生成一个简单的博客网站，当然如果你有心，还可以让他更强大，下面就来简单记录下在Github上建立Hugo站的方法。
<!--more-->
## 安装Hugo

[Hugo]的安装很简单，按照官网介绍即可，在Mac上可以选择source安装，或者brew。

    {{  brew install hugo }}

需要注意的是，Hugo是基于Go开发的，因此需要Go的环境来支持，如何安装[Go] 请猛戳［安装Go］

## 使用Hugo建立你的博客

Hugo建立网站只需要一个命令：

    {{  hugo new site myblog }}

建立完成后就可以马上在本地将Server运行起来查看效果：

    {{ hugo server -w -t hyde }}

这里是使用了hyde这个主题。

## 创建你的第一篇文章

可以通过下面的命令来创建文章：

    {{ hugo new post/fist.md }}

打开并使用markdone语法来编写文章就可以啦：
```
 +++
 date = "2015-02-18T00:38:59+08:00"
 title = "Setup Hogo on Github How to" 
 tag = ["hugo", "howto"] 
 categories = ["howto"]
 +++

 The First

 Hello ....
```

## 入驻Github

思路很简单，建立两个repo，一个用来储存Blog的Hugo源文件，包含md，模版等，另一个repo则只包含Hugo生成的Public目录，即静态网页内容，而我们访问的就是这个静态网页的repo。


[Go]: <https://golang.org/>
[Hugo]: <http://gohugo.io/>
[安装Go]: <https://golang.org/doc/install>


