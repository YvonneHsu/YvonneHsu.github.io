---
layout: post-series
title: Beginning with - pwd, ls and cd
author: aditya
excerpt: "A terminal window allows the user access to a text terminal and all its applications such as command-line interfaces (CLI) and text user interface (TUI) applications. Lets analyze a few basic applications of using the Terminal."
category: howto
series: Basics of Terminal
tags: [terminal,linux,unix,os]
comments: true
image: 
   feature: Introduction to Terminal.png
   thumb:
---

{% include _toc.html %}

In this section we will cover all the techniques to get familiar and comfortable with using Terminals.

## Introduction

I would be lying if I said 

>	I loved using terminals as soon as I started using them.

Because my past experience with OS had all GUI based (Windows), I had never voluntarily opened command prompt or cmd (Equivalent to terminal of Linux).
It felt like a whole new challenge. All I'm doing here is to help people feel comfortable while using terminal.

## Prerequisite

Linux, Unix, Android (Use [terminal emulator](http://play.google.com/store/apps/details?id=jackpal.androidterm) and [Busybox](http://play.google.com/store/apps/details?id=burrows.apps.busybox)) or even Windows (Use [Cygwin](https://www.cygwin.com/))

## Basics 

Linux and Unix terminals are case sensitive, that is 

* **TECHYUGA** 
* **techyuga** 
* **TechYuga** 

are all different. 
The ~ (tilde) symbol is shortform of path to your Home directory.
And / (root) is the first or top most directory. 
To bring out the terminal press Ctrl+Alt+t (Works for most of the Linux distributions). 
Use up key to see your previous commands. Make it a habit to use terminal as much as possible.

## The pwd command

The most basic command, and quite useful.
The pwd command when entered in the terminal gives back your current working directory.
pwd stands for "Print Working Directory". If you think you are lost and don't know where you are, then use this command.
![pwd in use](/images/contentimages/IntroductiontoTerminal/1pwd.png "pwd in use")

## The ls command

The ls command lists the files in that location. In case you forgot what the file name is, then use this command. 
![ls in use](/images/contentimages/IntroductiontoTerminal/2ls.png "ls in use")

## The 'Tab' key

While you are typing a command or a file name, if you forget the complete name use Tab key to auto-complete.
Believe me, after learning this you will press Tab more often than you need.

## The cd command

The cd command is used to change directories. There are two ways you can do this 

### Absolute pathname

If you know which directory and its complete path from root (/), then you can use this method. 
Using Tab key gives list of all the directories present from that particular directory. And can also be used to auto-complete directory names. 
Use cd ~ to go to home directory.
![from root to Music](/images/contentimages/IntroductiontoTerminal/3absolute.png "from root to Music")

### Relative pathname

To change directories, you have to find where you are currently standing with help of pwd.
And then again change directories with cd command till the specific directory is reached. 
![from home to Music](/images/contentimages/IntroductiontoTerminal/4relative.png "from home to Music")

Lets look at the special characters '..' and '.'

The '..' refers to the parent of whatever directory you are currently in.
Its like one level closer to root directory.
![usage of .. operator](/images/contentimages/IntroductiontoTerminal/5..operator.png "usage of .. operator")

The '.' refers to the current directory.
![usage of . operator](/images/contentimages/IntroductiontoTerminal/6.operator.png "usage of . operator")

## Did you Know?

You can use Ctrl+m insted of ENTER key. These are called as 'Control Characters'. Some other Control Characters are 
Ctrl+h for BACKSPACE, Ctrl+d to indicate end of input file, Ctrl+c to BREAK (Stop running program immediately).

## Summary 

Commands used
{% highlight text %}
pwd
ls
cd
|-- Absolute 
|-- Relative
Tab -- auto-complete
{% endhighlight %}

Congrats you can now go to any directory you want in the system.<br/>
Please use the comment section responsibly, I'll try my best to reply.<br/>
This is one of the many posts for using the Terminal.<br/>
Check this website for more useful posts regarding Linux and JAVA programming.<br/>
