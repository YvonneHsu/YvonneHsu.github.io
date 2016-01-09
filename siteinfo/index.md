---
layout: page
title: Complete Documentation of this Website
excerpt: Full Documentation about the Website for both authors and site maintainers
tags: 
  - HowTo
  - Reviews
  - Software
  - Programming
comments: true
share: false
image: 
  feature: deer.jpg
published: true
---

{% include _toc.html %}

**Documented by:** Manu Mathew

Hello!! If you are reading this, chances are that I instructed ( or begged :sweat_smile: ) you to do so. If not, I'm proud of you :blush:. Well, the fact is that you are here. Let's just dive right into the topic. I am motivated to setup this documentation as I could see the functioning of the website seemed a bit much on the geeky side of things. Trust me, I've been in similar situations. I cannot guarantee you complete sanity in understanding the nooks and corners of this website unless you try and do stuff for yourself. This guide is aimed at two class of stakeholders of the site:

- Article Authors
- Website Maintainers

But if you think you do not belong to either of these, then stick around you may want to help us. Let's first start with setting up the website.

**Setting up the Website? Isn't it already setup?**<br/>
Yes. The site is setup online for all our visitors. But you are not a visitor, you are now a part of the Tech Yuga Organization, which means your role is beyond just reading the articles on our site. You can now write articles or do site maintenance yourself. In order to do so, you need to have a copy of the website on your local computer. And that is what I meant when I said setting up the Website.
{: .notice }

## Setting up the Website
The most basic qualification to be a part of the Tech Yuga Organization is having an account at [GitHub](http://github.com "Register youself at GitHub"). 

Once you have done that, the next step is to join the [Tech Yuga Organization](http://github.com/TechYuga) at GitHub. That part is upto me. Just let me know when you finish creating a GitHub account, I'll invite you into the Tech Yuga Organization.

You are OK to get started now, but we are not done yet. The reason I say this is because you can use GitHub itself or services like [prose.io](http://prose.io) to start writing articles. But articles in our website are much more than just text. Articles in our website contain feature images, categories and tags in addition to text content. To create and interact with these elements, you need to clone the website repository to your local system. Basic requirements for this is to have a Linux system. I recommend using Ubuntu linux as it is easy to Setup and use. Once you have done this, open the terminal and do the following:

- Create a Project directory to store the repository.
{% highlight bash %}
$ mkdir project
{% endhighlight %}

- Navigate to this directory.
{% highlight bash %}
$ cd project
{% endhighlight %}
- Clone the repository. 
{% highlight bash %}
$ git clone http://github.com/TechYuga/techyuga.github.io
{% endhighlight %}

