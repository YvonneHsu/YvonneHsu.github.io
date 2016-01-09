---
layout: post
title: Top things to do after installing Elementary OS Luna 0.2
excerpt: "Here's a comprehensive list of top things to do after installing Elementary OS Luna 0.2"
category: howto
tags: [linux,os,work-around,terminal]
comments: true
image: 
   feature: Top things to do after installing Elementary OS Luna 0.2.jpg
   thumb:
---

{% include _toc.html %}

So you have now installed Elementary OS, huh? Don't you feel it's missing something?

It certainly does miss a lot of features users usually expect from a normal Ubuntu distribution. Let's try filling up that gap by doing some stuff. I present to you top things to do after installing Elementary OS Luna 0.2.


### 1. Website To-Do List

The Elementary OS Update website has posted an exhaustive list of things to do after installation. It is an excellent place to start with. Click [here](http://www.elementaryupdate.com/2013/08/top-things-to-do-after-installing-luna.html "Top Things To Do After Installing Luna") to read this.

**UPDATE**: The Elementary Update website is unavailable at the moment for [unknown reasons](https://plus.google.com/102580688829137570296/posts/KRSH8s7mJrY). You can however use [this link](http://elementarytips.blogspot.pt/2013/08/top-things-to-do-after-installing-luna.html) to complete this step.

### 2. Install the ubuntu-restricted-extras package
The ubuntu-restricted-extras package installs various packages not included by default on an ubuntu distribution disc because of legal restrictions like copyright issues. This includes support for various audio/video formats, Flash plugin, Microsoft Fonts, LAME (to create compressed audio files), and DVD playback.

To install, use the Software Center or press Ctrl+Alt+T to open the Terminal, type the following command:
{% highlight bash %}
$ sudo apt-get install ubuntu-restricted-extras
{% endhighlight %}

### 3. Install Synaptic Package Manager and GDebi Package Installer
Synaptic Package Manager is a Package Management Utility for installing Applications. It can be considered as an immediate replacement for the Software Center. To install Synaptic, press Ctrl+Alt+T to open Terminal, and type:

{% highlight bash %}
$ sudo apt-get install synaptic
{% endhighlight %}

GDebi Package Installer is a Debian Package Installer. It helps you install *[.deb packages](/pc/2013/01/29/packaging-deb-files.html ".deb files")*, which can be used to install several packages with a single click. To install GDebi, press Ctrl+Alt+T to open Terminal, and type:

{% highlight bash %}
$ sudo apt-get install gdebi
{% endhighlight %}	

### 4. Install Gnome System Monitor
A System Monitor Application is a handy tool to monitor system resources and do process management. To install this, press Ctrl+Alt+T to open Terminal, and type:

{% highlight bash %}
$ sudo apt-get install gnome-system-monitor
{% endhighlight %}

### 5. Install an Office Application
Elementary OS Luna does not come with any pre-installed Office Applications. Let's now install an Office Application for Luna.

#### Solution 1: LibreOffice    
LibreOffice is the default Office Application for most Linux Distributions. It supports all the Open Document Formats as well as the Microsoft Office Documents. It is an Open-Source Product. LibreOffice comes with not only Word Processing, Presentation and Spreadsheet applications, but also drawing tools, math tools, and database management tools. LibreOffice can be found in the Software Center.

#### Solution 2: Kingsoft WPS Office      
Kingsoft WPS Office is a proprietary Office Solution available in Linux, which comes with the three basic Office applications: Word Processing, Presentation and Spreadsheets (hence the name WPS). It supports its own formats along with Microsoft Office formats. Visit the Kingsoft Office [website](http://wps-community.org/download.html "Kingsoft WPS Office Download") to download it. Download the package with .deb extension, and open it with GDebi Package Installer to install it.

### 6. Install Drawing and Image Manipulation Applications
MyPaint is an excellent free-draw application with lots of brushes. To install MyPaint, press Ctrl+Alt+T to open Terminal, and type:

{% highlight bash %}
$ sudo apt-get install mypaint
{% endhighlight %}

If you are a Linux User, you cannot simply search around for Image Manipulation Tools without trying out GIMP, which is a Professional Tool for creating and editing Images, much like Photoshop or in many aspects better. To install GIMP, press Ctrl+Alt+T to open Terminal, and type:

{% highlight bash %}
$ sudo apt-get install gimp
{% endhighlight %}	

### 7. Install a Disc Burning Tool
A Disc Burning Tool is a vital piece of Software for any OS. K3B is an excellent Disc Burning Tool for Linux. To install K3B, press Ctrl+Alt+T to open Terminal, and type:

{% highlight bash %}
$ sudo apt-get install k3b
{% endhighlight %}		

### 8. Install a Bit-Torrent Application
Whether to install various Linux ISO Images or download movies, a torrent file is the preferable method for the masses. To download content using a torrent, you need a Bit-Torrent Application such as uTorrent, Transmission, qBittorrent,etc. qBittorrent seems to be a nice choice for Linux as it resembles the familiar uTorrent Application. To install qBittorrent, press Ctrl+Alt+T to open Terminal, and type:

{% highlight bash %}
$ sudo apt-get install qbittorrent
{% endhighlight %}

### 9. Install an IRC Client
An IRC Client might serve as a goto tool when you feel the urge to chat with someone on an IRC channel or contact your Distro community when you need help with something. XChat is an excellent IRC Client for Linux. To install XChat, press Ctrl+Alt+T to open Terminal, and type:

{% highlight bash %}
$ sudo apt-get install xchat
{% endhighlight %}

### 10. Sit back and enjoy!
You've done it! You have made Luna marvelous. These steps should make your life easy around Luna. All that is left is to enjoy using Luna. Have a great time using Luna! Cheers..

**Note:** I might have missed out something somewhere. Please share your opinions and suggestions with us through comments.