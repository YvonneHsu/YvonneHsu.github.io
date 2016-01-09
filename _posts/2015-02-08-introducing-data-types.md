---
layout: post-series
title: Introducing Data Types in Java
series: Java Programming
excerpt: "There are various types of data. Let's look at the different types of data (data types) present in Java"
author: ashwin
comments: true
category: programming
tags: [java]
image:
   feature: introducing-data-types.jpg
   thumb:
---

{% include _toc.html %}

Data type! (Sounds complicated?) Don't worry it's nothing to be worried about. By the time you finish reading this post you'll know what a data type is, how many types are there, and how to use them. Why wait? Let's dive right in!

Let's suppose you ask somebody for their phone number and they reply saying my phone number is `heyashwinthisismyphonenumber`. What will you say in response?. 

> Hey! That's not a phone number! 

Why do you say this? This is because you know that you were expecting a series of numbers to be the appropriate response to the question. Now in computer programming terms the phone number can be thought of as a data type. Nothing else other than phone numbers can be put into a variable of type phone number.

Similarly in Java we have eight basic data-types (also called primitives). The eight data-types are: 

- boolean
- char
- byte
- short
- int
- long
- float
- double

Let's look at each of these in more detail:

### boolean
Any variable that is declared to be of this type (boolean) can store one of two values namely `true` or `false`. No other data can be stuffed into a boolean variable. <br/>
Syntax for creating a boolean variable:

{% highlight java %}
boolean variableName;
{% endhighlight %}

Now let's create a variable called `booleanVariable` and assign it the value `true`:

{% highlight java %}
boolean booleanVariable = true;
{% endhighlight %}

Any conditional operator also returns a boolean value depending on the outcome of the expression! We'll see this in the next post on operators and expressions!
{: .notice }

###int
You guessed it! It's an **int**eger. Variables of type int store integer values. Integers are exactly what we know them to be! However there is a limitation to this data-type, int can only store values of the range `-2147483648` to `+2147483647`. Any attempt to store values out of this range will result in a compile-time error.

There are no unsigned integers in Java!
{: .notice }

Now let's create a variable `a` of int type and assign it a value of `5`:

{% highlight java %}
int a = 5;
{% endhighlight %}

###byte
A byte is similar to an int. The two main differences are the range of values that a byte variable can hold and the number bits that a byte variable uses. A byte variable uses only 8-bits to represent values and because of this the range of a byte variable is restricted to `-128` to `+127`.<br/>
Syntax for creating a byte variable:

{% highlight java %}
byte variableName;
{% endhighlight %}

Now let's create a variable and assign it a value:

{% highlight java %}
byte variable = 100;
{% endhighlight %}

###short
A short too is similar to a byte. The two main differences are the range of values that a short variable can hold and the number of bits that a short variable uses. A short variable uses 16 bits to represent values and this causes the range of a short variable is limited to `-32768` to `+32767`.<br/>
Syntax for creating a short variable:

{% highlight java %}
short variableName;
{% endhighlight %}

Now let's create a variable and assign it a value:

{% highlight java %}
short variable = 1000;
{% endhighlight %}

###long
Sometimes there is a need to have a very large integer and by large I mean huge!! **long** to the rescue. A variable which is of type long uses 64 bits to represent values as a result the range of a long variable lies between `-2^(63)` to `+(2^(63))-1`. This should be enough right? :stuck_out_tongue:<br/>
Syntax for creating a long variable:

{% highlight java %}
long variableName;
{% endhighlight %}

Now let's create a variable and assign it a value:

{% highlight java %}
long variable = 888888888;
{% endhighlight %}

###char
Doesn't it seem like 'char' is actually a short-form for something? What on earth could it be? Stop guessing it's short for **char**acter :smile:. A character is a single letter of the Java alphabet. Java alphabet? What's that? 

Java uses Unicode character set. 
{: .notice }

A character is stored as a 16-bit unsigned integer but is represented as a character when displayed. All the letters in the Java alphabet have a 16-bit number associated with them. For example the character `a` in decimal has a value of `97`.<br/>
Since characters are associated with integers it's not uncommon to see characters used in expressions. All **char** types need to be enclosed within singles quotes `' '`.<br/>
Syntax for creating a char variable:

{% highlight java %}
char variableName;
{% endhighlight %}

Now let's create a variable and assign it a value:

{% highlight java %}
char myFirstCharVariable = 'a'; 
{% endhighlight %}

###float
Variables of this type will have a floating point. What does floating point mean? It means decimal point!! I'm sure all of us have used numbers of the form 3.14, 5.6,etc. Numbers of this kind are called as floating point numbers. float uses 32 bits to hold values. All numbers in Java of the form x.y are treated as double types (double is explained next). So to specify to the compiler that this value is a float and not a double we append 'f' to the floating point value.<br/>
Syntax for creating a float variable:

{% highlight java %}
float variableName;
{% endhighlight %}

Now let's create a variable and assign it a value:

{% highlight java %}
float variable = 2.04f; 
{% endhighlight %}

###double
Variables of type double are similar to those of float. The difference is the number of bits that double uses to represent values. float uses 32 bits whereas double uses 64 bits. This means that double will have a very high precision. Therefore double is used in applications or calculations where high precision is necessary. All numbers in Java of the x.y are by default treated as double values.<br/>
Syntax for creating a double variable:

{% highlight java %}
double variableName;
{% endhighlight %}

Now let's create a variable and assign it a value:

{% highlight java %}
double variable = 2.000004;
{% endhighlight %}

Now that we know what data types are, let's put variables inside our class:

{% highlight java %}
class PrintingPress {
	int numberOfPages;
	float price;
}
{% endhighlight %}

Now,we have created a class that has two properties namely numberOfPages (an integer) and price (a float).<br/>
In the next article we'll see how to create objects and learn about operators.
