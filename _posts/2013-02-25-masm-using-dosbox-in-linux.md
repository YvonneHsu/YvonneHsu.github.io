---
layout: post
title: MASM using DOSBox in Linux
excerpt: "Learn how to use Microscoft Macro Assembler (MASM) in Linux using DOSBox"
category: howto
tags: [work-around,linux,dosbox,virtualization]
comments: true
image:
   feature: MASM using DOSBox in Linux.jpg
   thumb:
---
MASM (Microsoft Macro Assembler) is an Intel x86 Assembler used to compile and build programs written in Assembly level language. Like many other softwares from Micosoft, MASM is released for only DOS and Windows. So, for softwares like this to get working on other OSes, you need an emulator capable of emulating it using the available resources of the OS. Let us see how a DOS version of MASM can be emulated in Linux using the DOSBox Emulator.

* To get started, download MASM for DOS. Make sure you have the following files inside the masm folder:

	1. MASM.EXE
	2. TASM.EXE
	3. LINK.EXE
	4. EXE2BIN.EXE
	5. BIN2HEX.EXE
	6. DEBUG.EXE
	7. EDIT.COM
	8. TD.EXE

* Copy the masm folder to your Home Folder.
* Open a terminal and type the following command to install DOSBox in Linux:

{% highlight bash %}
$ sudo apt-get install dosbox
{% endhighlight %}

* Run DosBox once and exit out of it. This will create “.dosbox” folder in your home folder. Open that folder (This is a hidden folder, press Ctrl+H to unhide it) and double click on dosbox-x.xx.conf file.
* Go to the last line and add these lines, save and exit. You'll get the masm folder mounted as C: drive when DOSBox opens.

{% highlight bash %}
$ mount C: ~/
$ C:
{% endhighlight %}

Opening DOSBox will be like opening Command Prompt (cmd) in Windows from now on. You can start using MASM like you do in Windows. You don't have to redo all the above steps again at a later time.

* cd to masm folder like this:
{% highlight bash %}
$ cd masm
{% endhighlight %}	

There are many alternatives in Linux for MASM like nasm, yasm, etc. Try using any of these if you don't follow MASM.<br/>
So what are you waiting for? Get your program assembled in Linux today.