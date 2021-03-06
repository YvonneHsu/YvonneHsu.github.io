---
layout: post
title: Markdown 迷你语法指南
excerpt: "一份简版的 Markdown 入门手册"
author: Azeril
tags: [guide, ]
image:
  feature: windows.jpg
  credit: Azeril
  creditlink: http://azeril.me
---

{% include _toc.html %}


## Start

写作 Jekyll 博客使用的主要是两种语法：

* HTML
* Markdown


Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档，然后转换成格式丰富的HTML页面。 

一般我们使用 Markdown 语法。原因是语法简单，还有书写更快捷，可扩展性能也颇佳。

而日常使用 Markdown 最频繁的就这个几个语法：

* 标题
* 列表
* 引用
* 链接
* 图片

本篇就只介绍最常用的几个。更详细的指南可以直接查看文末的扩展阅读链接。

## 换行

讲这些之前先说一下换行。Markdown 里无论你前面空多少格，呈现效果里文字都是从行首开始的。

而如果换行，有两个方式，第一，在行末空两格，而后回车；第二，在行末两次回车，空出一行，再继续写新的内容。

## 标题

标题都是「#」开头，空一格，后接文字。GitHub 显示支持六级标题。一般三级使用就够了。

```
# 我是一级标题
## 二级标题啦
## 嗯，是三级标题咯
```

## 强调

强调分两种：

1. 斜体
2. 加粗

```
*比萨斜塔*  
**比萨**斜塔
```

显示效果如下：

*比萨斜塔*  
**比萨**斜塔

除了使用「*」之外，还可以用下划线「_」来起到同样的作用。

## 列表

列表分有序列表和无序列表。

有序列表/无序列表的语法形式是这样：

```
有序一点如何：

1.黑
2.凤
3.梨
```

```
生活好物~

* iPhone
* 乐泡移动电源
* Kindle
* 蚕丝围巾
* Lamy 钢笔
```

注意空格，列表与前面的内容间要空一行，不然语法将无法使用。

## 引用

**引用**在摘录笔记时比较常用。

语法形式如下（「>」后边，空一格后再添加具体内容）：

```
> 我希望你有时候能驻足于这个令你感到惊叹的世界。如果和你想象的生活不一样，我希望你能有勇气，重新启程。
> 
> ——本杰明·巴顿
```
或者

```
歌德曾说过：

> 最真诚的慷慨就是欣赏
```

呈现的效果则是这样：

> 我希望你有时候能驻足于这个令你感到惊叹的世界。如果和你想象的生活不一样，我希望你能有勇气，重新启程。
> 
> ——本杰明·巴顿奇事

或者

歌德曾说过：

> 最真诚的慷慨就是欣赏


## 链接

添加链接的常用语法是这样：

```
[Link Name](Link) 
```

```
[Google](http://google.com)
```

自动链接的形式则是这样

```
<http://paw.cat>
```

## 图片

链接的语法前加「!」(英文是感叹号)就是图片链接的形式了。当然，链接的网址必须是图片的链接才行。通常，我们称之为直链，也即图片的直接链接。

```
![Pic name](Pic link)  
```

```
![Instagram Pic](http://i.imgur.com/UKhrRrK.jpg)
```

效果是这样：

![Instagram Pic](http://i.imgur.com/UKhrRrK.jpg)

图床：图床是第三方服务托管个人上传图片，并提供图片外链，让我们在写博客文章时使用的方式。

常用图床： 

* [七牛云存储](http://www.qiniu.com/)
* [Imgur](http://imgur.com/)
* [Photobucket](http://s1381.photobucket.com/)

图床在上传图片后会提供一个图片的外链。我们可以利用外链把图片添加到自己的博文中加以显示。当然，其实图片也可以存储在 Github 自己的博客仓库里（比如博客的首页大图），但图片蛮占用空间（Github 项目空间为200 M）。因而最好是选图床托管图片。

## 其它语法

还有诸如代码区块、转义符一类的语法，以及每个语法的具体细节强调，这里就不多说了。自己慢慢摸索，也可以在具体写作时参考详细的 Markdown 语法指南。

扩展阅读：[Markdown 简明语法参考 - Microdust](http://azeril.me/blog/Markdown-Syntax.html)

## 博客图文模式

在博文中并排显示多张图片的技巧。仅作了解：

[Sample Post Images](http://paw.cat/Sample-Post-Images.html)