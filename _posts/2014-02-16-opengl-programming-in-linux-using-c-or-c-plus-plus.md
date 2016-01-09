---
layout: post
title: C and C++ OpenGL Programming in Linux
excerpt: "Learn how to use Linux for OpenGL Programming using C/C++ with opengl/glut libraries"
category: howto
tags: [c,c++,linux,unix,terminal,work-around]
comments: true
image:
   feature: C and C++ OpenGL Programming in Linux.jpg
   thumb:
---

{% include _toc.html %}

This article deals with setting up a debian based Linux system like Ubuntu to do OpenGL Programming. We'll be using OpenGL gl/glu/glut libraries to accomplish this task. Here is a step-by-step tutorial of preparing the system for OpenGL programming, writing our first program and compiling it. 

### Installing the Build Essentials
Build essential is a package containing a set of programming tools like compilers. We'll need a C/C++ compiler that must be used to compile our programs. To install this package, open a terminal ( Ctrl+Alt+T ) and type:

{% highlight bash %}
$ sudo apt-get install build-essential
{% endhighlight %}	

### Installing the OpenGL Libraries
After the build essentials are installed, it's now time to install the OpenGL libraries. To install them, type the following command in terminal:

{% highlight bash %}
$ sudo apt-get install libglu1-mesa-dev freeglut3-dev mesa-common-dev
{% endhighlight %}
    
### Writing our First Program
Now that the system is ready for OpenGL programming, it's now time to write our first program. [Here](/documents/scc_program.cpp) is a Program for Spinning Color Cube. Save the program to the location of your choice.

### Compiling and running the program
To compile the program, from the directory when your program is stored, type the following command in terminal:

{% highlight bash %}
$ g++ scc_program.cpp -lglut -lGLU -lGL -Wall -g
{% endhighlight %}

If you are compiling a C program instead, replace *g++* with *gcc*. Here, the -lglut, -lGLU and -lGL tags are used to invoke the OpenGL libraries, -Wall tag shows all warnings and -g tag will help you in debugging the program.

To run the executable program, type:

{% highlight bash %}
$ ./a.out
{% endhighlight %}

![Output of Spinning Color Cube Program](/images/contentimages/CandC++OpenGLProgramminginLinux/1.png)

You should now see a spinning color cube that spins on different axis on different mouse button clicks. If you see this, then Kudos!!! You have successfully run your first program.
