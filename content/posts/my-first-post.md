---
layout: post
tags: ["Say Hi","Vno"]
title: "Hugo搭建个人博客教程"
date: 2022-11-20T18:36:17+08:00
math: false
draft: true
---

## **前言**

经过种种尝试，还是决定选择了Hugo作为了搭建个人博客的框架，Hugo是目前可以搭建个人博客的框架中部署最快的，而且坑也相对很少，不过还是有的，近几天折腾了不少东西，也终于算是初步搭建完了Hugo+Zoo主题的[个人博客](https://link.zhihu.com/?target=https%3A//blog.calvinhaynes.top/)

在本文中我会讲解部署的详细过程，也会科普一些部署中的原理，毕竟我也刚刚接触，所以有些说的不对的地方也希望评论区的大佬来勘误，谢谢啦。

如果遇到部署问题，欢迎在评论区打出你的问题，我和知乎这个优秀社区的所有人都有可能回答你的疑问哦，本文如果对你有帮助的话，还希望多多点赞收藏转发，谢谢啦。

## **1 - 使用Hugo创建静态网站实战**



### **1、安装Hugo**

博主用的是Windows系统，所以安装过程中我会基于Windows进行讲解，有关其他操作系统的安装方法可以参考官方的[文档](https://link.zhihu.com/?target=https%3A//gohugo.io/getting-started/installing/)

Windows下的Hugo安装我推荐使用chocolatey包管理器进行安装，接触过Linux的朋友们都知道，Linux的各种包管理器，利用命令行就可以实现包的更新，删除等操作，Windows下也有类似的包管理器就是chocolatey了。



**安装过程详解**

- 安装chocolatey包管理器：在[官网](https://link.zhihu.com/?target=https%3A//chocolatey.org/)点击 `Install Now` 即可下载
- 命令行中敲入`choco --version`，如果显示版本号证明你的 chocolatey 已经安装完毕，如果有误请检查环境变量
- 命令行中安装hugo：
  choco install hugo -confirm
  安装hugo-extended（扩展版本）：
  choco install hugo-extended -confirm
- 检查hugo是否安装成功：命令行中敲入`hugo version`