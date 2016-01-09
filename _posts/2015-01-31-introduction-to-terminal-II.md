---
layout: post-series
series: Basics of Terminal
title: Moving on with - mkdir, nano, cat, man and using redirections
author: aditya
excerpt: "Learn how to create source program files and manage them, use redirections and access manual pages."
category: howto
tags: [terminal,linux,unix,os]
comments: true
image: 
   feature: Introduction to Terminal.png
   thumb:
---

{% include _toc.html %}

In this section let's learn how to create and manage directories and text files, also about manuals for commands.

## The mkdir command

This command is used to create new directories. 

![Create a directory New in Documents](/images/contentimages/IntroductiontoTerminal/post2/1mkdir.png "Create a directory New in Documents")

mkdir command followed by a number of directory names creates multiple directories. 

![Create multiple directories New1, New2 in Documents](/images/contentimages/IntroductiontoTerminal/post2/2mkdir.png "Create multiple directories New1, New2 in Documents")

No need to go to that specific parent directory to create new directories, use Absolute pathname. (Easy right :smile: )

![Create multiple directories using Absolute pathname](/images/contentimages/IntroductiontoTerminal/post2/3mkdir.png "Create multiple directories using Absolute pathname")

To create subdirectories or directory tree in one command use option -p. Remember the '.' operator?

![Create subdirectories or directory tree](/images/contentimages/IntroductiontoTerminal/post2/4mkdir.png "Create subdirectories or directory tree")

## Creating files (nano)

Now we know how to create single and multiple directories anywhere we want. It looks kinda boring let's add some files in them.
To create text files we need editors, we have lots of editors starting from simple Command line 'ed' to Graphical 'Sublime'.<br/>
For this post I'll be using a simple editor called 'nano'.

To create a new file we have the command nano followed by file_name.extension, like source.cpp, Sample.txt, etc.

![Create a new file temp.txt](/images/contentimages/IntroductiontoTerminal/post2/5nano.png "Create a new file temp.txt")

This is what nano looks like when inside. (Amazing!) 

![Inside of nano](/images/contentimages/IntroductiontoTerminal/post2/6nano.png "Inside of nano")

You can start typing here. And when done use Ctrl+o to save, change name if required and press ENTER. 

![Saving the file](/images/contentimages/IntroductiontoTerminal/post2/7nano.png "Saving the file")

And finally Ctrl+x to exit.

Obviously the editor is massive and has lots and lots of options and I can't cover all the options here.
Here is the link to its official documents [here](http://www.nano-editor.org/docs.php).

Other editors are [Link to wikipedia](http://en.wikipedia.org/wiki/List_of_text_editors)

This is just my suggestion, find your Perfect Editor and stick with it. Its equally important to be very loyal and faithful to it.
This is very important to learn and use the editors to master them. Programmers All the Best! 

## The cat command

cat - shorthand for concatenated.
Simplest printing command and it prints the contents of all file_names given in arguments.

![cat command with two files](/images/contentimages/IntroductiontoTerminal/post2/8cat.png "cat command with two files")

## The man command

The command man is shorthand for manual. This command followed by a command opens the manual of that command. Remember to check it before using a relatively new command. Anything followed by - or -- is an option. 

![Opening manual of ls](/images/contentimages/IntroductiontoTerminal/post2/9man.png "Opening manual of ls")


![manual of ls command](/images/contentimages/IntroductiontoTerminal/post2/10man.png "manual of ls command")

Press q to quit.

## Standard Input, Output and Error

Imagine the whole input, output and error as plumbing in a Unix system. We have three different pipes connected to shell, lets call them

* **stdin** 
* **stdout** 
* **stderr** 

And each of the files are designed in such a way that they can allow a character stream(Water) to flow in only one direction.
stdin takes water **in** to the shell. stdout and stderr takes out water **out** of shell. 

By default stdin pipe is connected to Keyboard, and both stdout and stderr pipes are connected to terminal display(for simplicity lets call this as Monitor).
It looks like this 

![Default](/images/contentimages/IntroductiontoTerminal/post2/11red.png "Default")

You have the power to change the piping as you like. So stdout can be connected to a file called 'Temp'. Like this

![stdout connected to Temp file](/images/contentimages/IntroductiontoTerminal/post2/12red.png "stdout connected to Temp file")

To achieve this we can use the '>' operator. Note using '>>' will append characters instead of truncating the file.
An example  

![Using redirection operator > to save all file names in Temp file](/images/contentimages/IntroductiontoTerminal/post2/13red.png "Using redirection operator > to save all file names in Temp file")

You can see that Temp is created first only then ls is executed. 

Similarly you can redirect stdin pipe to accept character stream as text input from a file like 'Message'

![stdin connected to Message file](/images/contentimages/IntroductiontoTerminal/post2/14red.png "stdin connected to Message file")

To make this possible we have '<' operator.
An example 

![Using redirection operator < to get list of files present in Documents directory](/images/contentimages/IntroductiontoTerminal/post2/15red.png "Using redirection operator < to get list of files present in Documents directory")

We have '2>' for stderr. 

![Using redirection operator 2> to get error messages to a file Parent](/images/contentimages/IntroductiontoTerminal/post2/16red.png "Using redirection operator 2> to get error messages to a file Parent")

* **>** -- stdin
* **&gt;&gt;** -- stdin append
* **<** -- stdout
* **2>** -- stderr

The applications of using this effectively will reduce workload quite considerably. As they say 

>	Practice makes a Person Perfect (PPP)

## Did you Know?

Want to copy from a terminal press Ctrl+Shift+c. To paste to a terminal use Ctrl+Shift+v.

## Summary 

Commands used
{% highlight text %}
mkdir
nano (Editor)
cat
man
All standard redirections
{% endhighlight %}

Congrats you now know to create directories, make different files, know how to read a manual and how redirection works
