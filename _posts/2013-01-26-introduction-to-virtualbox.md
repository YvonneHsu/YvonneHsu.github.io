---
layout: post
title: Introduction to VirtualBox
excerpt: "A brief introduction to a great Virtualization software called Virtualbox."
comments: true
category: software
tags: [virtualization,os,work-around,communication]
image:
   feature: Introduction to VirtualBox.jpg
   thumb: 
---
Virtual Box (VBox in short) from Oracle is a great technology that helps us to install multiple operating systems on a machine and run them side by side. Hence it is called a Virtualization Software.
It allows any number of operating systems to be installed using it, the only limitations being Free Space and processing capacity.

It achieves this functionality by the concept of shared resources. The operating system in which VirtualBox is installed is called as the Host Operating System.  The operating systems which are installed in VirtualBox are called Guest Operating Systems. The Host OS shares its resources with VirtualBox which is utilized by the Guest OSes which are running.

Files and Network can be synced between the Guest OS and Host OS. Devices like USB and DVD drives can also be shared between the Guest OS and Host OS. A Virtual Partition or Hard Drive is created when you create a Guest OS using VirtualBox. These Partitions are considered as individual files on the Host OS. As it is not concerned with anything inside the Host OS, it is perfectly safe to test OSes in VirtualBox, play with things and delete them later. Thus VirtualBox can also be considered as a SandBox to carry out your tests on OSes.

VirtualBox is available for download in most popular platforms like Linux, Windows and Mac OS X. Check your Software Center or go to the VirtualBox [website](http://virtualbox.org "VirtualBox Website") to download and install your copy of VirtualBox.