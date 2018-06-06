---
layout: post
title:  "Taking Command"
date:   2018-06-04
excerpt: "A Beginner's Guide to Using the Command Line"
image: "https://image.ibb.co/edTov8/Beginner_Command_Line.png"
---

Today was all about breaking down basic command line in a way that any beginner could understand.
The __command line (or terminal)__ is a faster and much more powerful way to maneuver in your operating system than the _graphical user interface (GUI)_ we have all come to rely on so much. It is a less intuitive and uglier way of working with your operating system, but you can do a lot more with it than a GUI! In this post I will cover these basic maneuvers in the command line:
*   navigation
*   creating / removing directories and files
*   moving, copying and pasting things
The end aim is to be ready to utilise the command line to execute Python scripts.

## ‘You've got to find yourself first. Everything else'll follow.’ - Charles De Lint

You may or may not know that your operating system functions as a tree-like system, with everything growing from the __root__ directory. As sub-directories and files are added they grow along an _absolute path_. Each additional level along the tree is added as a "/".
You may assume that we would therefore start in the __terminal__ at the __root__ as our default. However you would be wrong.

By default, you will begin at the __home__ directory (also known as __~__). If we were to write out the default _absolute path_ it might be something like: _root/users/wendy/_
You are already in the branches of that tree!

_Why don't we default to the root directory?_
It is actually a very bad idea to start running things directly from the __root__. __Root__ allows for more access than a standard user needs and many of the features that make your account more secure will no longer be in place. Think of it another way, when you log in as your own user account, programs you run are restricted from writing to the rest of the system – they can only write to your __home__ folder. You can’t modify system files without gaining __root__ permissions. This helps keep your computer secure.

## 'All you need is the plan, the road map, and the courage to press on to your destination.' - Earl Nightingale

So now that we know where our home is, how do we know what else is in this tree? There are a few commands that can help. The first is __pwd (print working directory)__ . When entered in the terminal it will look something like this:

    :~ $ __pwd__
    _/Users/Wendy_

With __pwd__ command we can see the absolute path to our current position in the directories. It is a good way to look back on the path.

We can also use the __ls (list)__ command to view a list of a directory.
TBC....
