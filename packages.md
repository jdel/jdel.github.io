---
layout: default
title: Jdel.org - Synology Packages
---

Synology Packages
=================

Throughout the years I have been using different Synology NAS devices, I wrote many scripts to get it to do some work for me. After a few OS updates that destroyed every custom script I had every time, I started packaging my own scripts so they could survive a system upgrade.

As I couldn't find anything publicly available, this was quickly followed by [sspks](https://github.com/jdel/sspks/), a Simple Synology SPK Server. It has been reverse engineered from analyzing HTTP traffic from and to the official synology package server at the time.
sspks doesn't require a database, it uses the INFO and png file from the SPK. It's an old and dirty php script, written on-the-go, but it does the job.

If you are also developing your packages and are looking for an easy way to host them on your Synology NAS, don't look further, fork [sspks](http://github.com/jdel/sspks/) on github, make it better if you wish, and start using it.

I recently started having a look at cross compiling packages thanks to the superb [spksrc](https://github.com/SynoCommunity/spksrc/) framework used by SynoCommunity. 

I have forked spksrc in an [independent repository](https://github.com/jdel/syno-packages/) to host my own packages (that may not interest SynoCommunity). Software that I packages is available on my [SSPKS website](http://packages.jdel.org/).

Use my packages on your NAS
---------------------------

If you wish to help with the testing, or maybe because you need the functionality they provide, feel free to use my packages and report eventual bugs in the [issues tracker](https://github.com/jdel/syno-packages/issues/).

Just add the following source to your Synology Package Center:
``http://packages.jdel.org/``
