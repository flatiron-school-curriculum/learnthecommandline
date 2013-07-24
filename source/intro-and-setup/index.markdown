---
layout: page
title: "Intro and Setup"
date: 2013-07-24 03:00
comments: true
sharing: true
footer: true
---

Welcome to your first steps in learning the command line! Over the next few
hours you will learn new tools and techniques to truely transform your computer
into the tool that you need to be a successful developer.

For this tutorial I will only be covering the Linux and OS X shell. This is
simply because that is all I know. If you are on Windows, something like [Cygwin](http://www.cygwin.com/ "Cygwin Homepage") 
may be good to try out.

Why should I learn the command line?
------------------------------------

Because it's an incredibly efficient tool for much of what you'll do as a
developer. The truth is, the command line doesn't allow you to do too much
more. It just allows you to do it all a lot faster and a lot better. Once you
are a programmer, your computer is now your tool. This new tool is definitely
harder to learn that a graphical user interface, but the speed and efficiency
gains are worth it.

Also most of the common programming tools out today expect a certain level of
familiarity with the command line.

Setup
-----

Everything you need is already installed. How awesome is that?

###OS X
Let's open up Terminal.app. Open up the Finder and navigate to Applications >
Utilities. Look for the Terminal app and double click. You're good to go!

###Linux
The way to get to the terminal is a bit different in the different
distributions. If you are using Ubuntu, just hit the Windows key and then type
in Terminal. Click on the first result. For other distributions just look in
the application menu, it will be there I promise.

How To Use This Guide
---------------------

All of my "code" samples will be in blocks that look like this:


```bash
$ ls
Desktop    Downloads  Library  Music     Public
Documents  Dropbox    Movies   Pictures  VirtualBox VMs
```

You don't need to write the ```$```. That's just the prompt and you will see
that or maybe a ```>``` in your terminal. 

Common Themes On The Command Line
---------------------------------

Many of the commands you'll be using were actually developed by the same
[group](http://en.wikipedia.org/wiki/GNU)
of people. Over time a general set of best practices have risen up and most
command line programs are very similar in how they work. You'll probably notice
this while going through the guide, but here are the big ones.

###Flags
To get different output from commands beyond the default you are going to want
to use flags. Flags, or switches as some people call them, are modifiers like
`-l` to existing commands. For example, to list the contents of a directory
you would type ```ls```. If you wanted a more detailed listing though, you type
```ls -l```. If you wanted both a more detailed listing and better file size
display you'd type ```ls -lh```.

###Directories
There are many operations that you'll want to apply to a bunch of files. Many
different commands like `cp` and `rm` allow the use of the recursive flag,
`-r`. This will go into all the subdirectories of the directory you supplied
and run that command. It's easier to explain with an example. Lets say your
directory listing was as follows.

    dir/
    |_subdir1/
    | |_fileB
    |
    |_subdir2/
    | |_fileC
    |
    |_fileA

if we ran `rm -r dir` everything in dir and all it's subdirectories would be
  deleted. Or if you run `cp -r dir dir2` would copy dir and it's contents to
  dir2. Make sense? Good.

###Wildcards
When perusing the internet you may notice people using the `*` character in
their commands. All this means is everything. So if you are in a directory
filled with files and do `rm *` it would be as if you ran `rm` on every single
item in the directory. This expansion works with every command. It's a feature
of the terminal.
