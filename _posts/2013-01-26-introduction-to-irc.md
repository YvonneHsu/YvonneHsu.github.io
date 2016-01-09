---
layout: post
title: Introduction to IRC
excerpt: "Learn what is IRC and how you can use it to chat online with anyone and everyone."
category: software
tags: [irc,communication]
comments: true
image: 
   feature: Introduction to IRC.jpg
   thumb:
---
{% include _toc.html %}
A Chat service without delays and flaws! IRC (Internet Relay Chat) is a protocol in the Internet Protocol Suite, serving as an application layer. It is used to send and receive information and messages across different IRC servers in real-time.

IRC servers have *networks* which may contain any number of *channels* (similar to rooms in a building) where people can communicate with each other. A channel may contain any number of users. Channels usually are designated a particular topic on which the users can communicate.

Each user must have a *Nick* (a Nick-Name) that can be used to address him/her in the network. Nicks must be registered with *NickServ* (an IRC service bot) to prevent other users from using that Nick. Registered Nicks will be given a password to login to use the Nick. Unregistered Nicks are only temporary which will be unavailable for use once another user registers it.

To use IRC, you need an IRC client. IRC clients are available for all major platforms like Windows, Mac and Linux. Android and iOS platforms are also supported. An exhaustive list of IRC clients can be found [here](http://en.wikipedia.org/wiki/Comparison_of_Internet_Relay_Chat_clients "Comparison of IRC Clients"). Download the one you want and start using it. Chatzilla is a Firefox plugin which provides an IRC client. [Mibbit](http://mibbit.com "Mibbit Chat Client") is a web-based IRC client which runs on any given Web Browser.

### Joining an IRC Channel

Joining an IRC Channel is very easy. All you need to know is what network you need to join, server address and server password (if any) and the channel. To get started let's join #tech-yuga channel at spotchat network. To do so, click [here](https://kiwiirc.com/client), choose a Nickname, give the channel as *#tech-yuga*. Click on *server and network*, give the server address as *irc.spotchat.org* and leave the rest as-is and click on start.

### Registering and using a Nick

To register a Nick first assign a nick to yourself, as shown below:

>		/nick <nick>

*Example: /nick foo* <br/> <br/>
After assigning the nick, register it with NickServ

>		/msg NickServ register <password> <email>

*Example: /msg NickServ register bar foo@bar.com* <br/><br/>
You have to confirm the email address. To do this, follow the instructions in the message sent to the email address.<br/>
Every-time you join a channel in a network with registered nick, you can login to your nick by typing:

>		/msg NickServ identify <password>

*Example: /msg NickServ identify bar*  <br/>             

### Don't forget to make friends         

IRC is all about making friends, joining conversations, doing projects together,etc. All these require high discipline and manners. Make sure you keep your manners by not flooding the channel with unwanted messages, troll and offensive usage of words.<br/><br/>
So what are you waiting for? Join an IRC Channel now and chat with your friends!