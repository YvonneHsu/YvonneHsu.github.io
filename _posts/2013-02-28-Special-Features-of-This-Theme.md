---
layout: post
title: 博客特性指南
excerpt: "Example and code for using link posts."
tags: [ ]
---



## Markdown 语法

写作 Jekyll 博客使用的主要是两种语法：

* HTML
* Markdown

一般我们使用 Markdown 语法。原因是语法简单，还有书写更快捷，可扩展性能也颇佳。

如果不熟悉，还是得先补课。详细版的语法指南可以查看：

* [Markdown 简明语法参考 - Microdust](http://azeril.me/blog/Markdown-Syntax.html)

## 文章目录概览 Overview

显示在网页右侧的导航条，会将文章的一二三级目录合成到一列，便于点击和跳转。适用于长文。

用法很简单，在博文正文开头（YAML 编码后，正文）添加以下代码片段，文章转化时会自动附加目录导航条：

`{% include _toc.html %}`


## 博客图文模式 A Post with Images

在博文中并排显示多张图片的技巧。仅作了解：

[Sample Post Images](http://paw.cat/Sample-Post-Images/)


## 文章链接 link posts

没什么特别的，在显示时直接在标题边上添加一个链接的图标。点击后可直接跳转相应的网页（方便收录博客之外的网页）。

This theme supports **link posts**, made famous by John Gruber. To use, just add `link: http://url-you-want-linked` to the post's YAML front matter and you're done.

> And this is how a quote looks.

Some [link](http://www.mademistakes.com) can also be shown.
 

## 多作者模式 Author Override

These `owner` variables were defined in `config.yml`

Start by modifying or creating a new `authors.yml` file in the `_data` folder and add your authors using the following format.

{% highlight yaml %}

```
# Authors

billy_rick:
  name: Billy Rick
  web: http://thewhip.com
  email: billy@rick.com
  bio: "What do you want, jewels? I am a very extravagant man."
  avatar: bio-photo-2.jpg
  twitter: extravagantman
  google:
    plus: BillyRick

cornelius_fiddlebone:
  name: Cornelius Fiddlebone
  email: cornelius@thewhip.com
  bio: "I ordered what?"
  avatar: bio-photo.jpg
  twitter: rhymeswithsackit
  google:
    plus: CorneliusFiddlebone
{% endhighlight %}
```

To assign Billy Rick as an author for our post. You'd add the following YAML front matter to a post:


```
{% highlight yaml %}
author: billy_rick
{% endhighlight %}
```