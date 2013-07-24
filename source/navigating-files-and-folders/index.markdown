---
layout: page
title: "Navigating Files and Folders"
date: 2013-07-24 03:57
comments: true
sharing: true
footer: true
---
Moving around and using files and folders is computing 101. Let's learn how to
do that without lifting your hand off the keyboard.

Your Current Directory
----------------------

First of all, let's find out where you are. Usually the command prompt has the
current directory built into the prompt. Here is mine.
```bash
~/Documents $
```
What is that squiggle? That squiggle (```~```) is called a tilda and signifies
your home directory. This is the where your Documents, Downloads, etc folder
lives. On OS X it's located in ```/Users/<username>``` and in Linux it's
located at ```/home/<username>.```

If your ever get lost in the course of your days work you can findout which
directory you're in by typing ```pwd```. ```pwd``` as in Print Working
Directory.
```bash
$ pwd
/Users/Joe/Documents
```

Listing Files
-------------
There isn't much to it. Just type ```ls```.
```bash
$ ls
Desktop    Downloads  Library  Music     Public
Documents  Dropbox    Movies   Pictures  VirtualBox VMs
```
If you would like a bit more information like file size and permissions just
add the ```-l``` flag.





