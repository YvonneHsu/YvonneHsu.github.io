---
layout: post
title: C and C++ Programming in Linux - Text Editors
excerpt: "Learn how to use Linux for C/C++ Programming like you do it on DOS/Windows."
comments: true
category: howto
tags: [c,c++,linux,terminal,work-around,dosbox,os,virtualization,unix]
image: 
   feature: C and C++ Programming in Linux - Text Editors.jpg
   thumb:
---

{% include _toc.html %}

Many C/C++ Programming IDEs are not available for download on Linux. Here, we cover the solutions in Linux.
Here are two solutions you could use:

-  C/C++ Programming using Gnome Terminal, Text-Editors and gcc command.

-  C/C++ Programming using your favorite MS-DOS based IDE in DosBox.             

## C/C++ Programming using Gnome Terminal, Text Editor and gcc command:

### Using the VI Text Editor:
(This section assumes that you have installed VI Editor, gcc and g++)<br/><br/>
1) Press Alt+F2, type gnome-terminal (or konsole in KDE) and press enter(return key). cd to the directory to which you want to store your C Programs.

{% highlight bash %}
$ cd Documents
{% endhighlight %}
2) Open the file with VI Editor. Use .c extension for C Programs and .cpp for C++ Programs (applicable throughout this tutorial page)

{% highlight bash %}
$ vi filename.c
{% endhighlight %}

3) You now enter the VI Editor. To start writing your Program, press Insert (Ins) key and start typing.
Once you are done, Press Escape (Esc) key, type the following without quotation marks to save and exit out of the VI Editor.

{% highlight bash %}
:wq 
{% endhighlight %}

You now come back to the Terminal screen.<br/>
4) To compile your C/C++ Program, use the gcc command with -o flag between the program filename and the executable filename. 

{% highlight bash %}
$ gcc filename.c -o output_filename.out
{% endhighlight %}

5) If there are any errors in the program, it will be displayed. You can go back to your program for editing and correct your errors by repeating steps starting from 2nd step again.<br/>
If there are no errors, an output file by name "output_filename.out" will be created.
To test the output, type “./output_filename.out” without the quotation marks. The output will be displayed on the terminal screen.

{% highlight bash %}
$ ./output_filename.out
{% endhighlight %}

**Note:**<br/> 
- use g++ instead of gcc to compile C++ Programs.<br/>
- typing "gcc filename.c" alone will result in an output file “a.out”. To test this output, type "./a.out" on the terminal prompt.<br/>
{: .notice}

**Advantages of this method:** <br/>
- Parallel programming can be performed which Linux and Unix based OSes are so good at doing.<br/>
- You don’t have to leave the Terminal screen for anything once opened.<br/>
{: .notice}

### Using GUI based Text Editors like Gedit/Kate:

(This section assumes that you have installed gedit or kate, gcc and g++)<br/><br/>
1) Open the folder in which you want your C Program to be created.<br/><br/>
2) Right click, select Create New Document > Empty Document.<br/><br/>
3) Rename it to your liking, let’s assume "filename.c"<br/><br/>
4) Double-click your file, and start editing in Gedit/Kate, save your program and exit.<br/><br/>
5) Press Alt+F2, type gnome-terminal (or konsole in KDE) and press enter(return key).<br/><br/>
6) cd to the directory in which you have stored your C Program.<br/>

{% highlight bash %}
$ cd Documents
{% endhighlight %}

7) Type this to compile your C/C++ Program:

{% highlight bash %}
$ gcc filename.c -o output_filename.out
{% endhighlight %}

8) If there are any errors in the program, it will be displayed. You can go back to your program for editing and correct your errors by repeating steps starting from 4th step again.<br/>
If there are no errors, an output file by name "output_filename.out" will be created. To test the output, type “./output_filename.out” without the quotation marks. The output will be displayed on the terminal screen.

{% highlight bash %}
$ ./output_filename.out
{% endhighlight %}

**Note:**<br/>
- use g++ instead of gcc to compile C++ Programs.<br/>
- Typing gcc "filename.c" alone will result in an output file “a.out”. To test this output, type ./a.out<br/>
- Templates do not exist in KDE (Ignore the first 3 steps), hence program files have to be created manually each time.<br/> 
{: .notice}

**Advantages of this method:**<br/>
- Parallel programming can be performed which Linux and Unix based OSes are so good at doing.
{: .notice}

## C Programming using your favorite MS-DOS based IDE in DosBox:

(This section assumes that you have DosBox and the required IDE (like Turbo C/C++) installed.)<br/><br/>
1) Copy the contents of the installed IDE (from Windows) to your Home Folder and rename the folder to C (just for ease).<br/><br/>
2) Run DosBox once and exit out of it. This will create “.dosbox” folder in your home folder. Open that folder and double click on dosbox-x.xx.conf file.<br/><br/>
3) Go to the last line and add these lines, save and exit.

{% highlight bash %}
mount C: ~/C
C:
cd bin
{% endhighlight %}

4) Run DosBox again and type tc.exe (or whatever the IDE name is). This will open your favorite IDE for editing. Type, compile and test your program in it.<br/><br/>

**Advantages:**<br/>
- You can use your favorite IDE for C/C++ Programming.<br/><br/>
**Disadvantages:**<br/>
- Parallel Programming abilities of Linux is not accessible.<br/>
{: .notice }
<br/>So, what are you waiting for? Test your C/C++ Programming capabilities on your favorite Linux distro!