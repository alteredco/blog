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

    :~ $ pwd
    _/Users/Wendy_

With __pwd__ command we can see the relative path to our current position in the directories. It is a good way to look back on the path thus far.

![ls can see all!](https://i.ibb.co/PMDj3FF/sauron.jpg#feature)

We can also use the __ls (list)__ command to view a list of a directory but unlike __pwd__, it will look into any directory we point it to (like Sauron's eye!). This command can be used to peer into other directories, _without moving_, as long as we know the _absolute path_ to that directory.

    :~ $ ls /Users/Wendy/Projects
    _hello-world_  _portfolio_  _blog_

This can be useful when we want to start moving around quickly and use our next command: __cd (change directory)__.

## 'We keep moving forward, opening up new doors and doing new things, because we're curious...and curiosity keeps leading us down new paths.' - Walt Disney

The great thing about the __cd__ command, like we have seen with the __ls__ command, is that you can navigate in two different ways: _absolutely_ and _relatively_.

Navigating _absolutely_ means you follow the _absolute path_ (remember this term from the beginning of this post?). Regardless to where you currently are, the _absolute path_ to a location will always remain unchanged. It is like an address.

Navigating _relatively_ means that you find the path _from_ your current location. This is like using sat nav to get around. In most circumstances, this is much quicker than typing out a full absolute path. For example, if we were in the /Users/Wendy/ directory and we wanted to get into /Projects/, rather than type out: root/Users/Wendy/Projects we can just do the following:

    :~ $ cd Projects

_*One useful tip is that_ __tab__ _will autocomplete paths._

Relative navigation can be described in terms of _parent and child_ relationships. Our operating system to be a bit like a family tree. The closer to the root, the farther back in family history we go. The directory before our current location would be the _parent_ directory. There is actually a handy technique for moving backward based on this concept. In the command line "__.__" stands for the _current_ directory. "__..__" therefore stands for the _parent_ directory. We can move backward one step by simply typing:

     :~ $ cd ..

Finally, we can return to our default location by typing:

    :~ $ cd

## 'The best way to predict the future is to to create it.' - Peter Drucker

Your newfound powers in the command line can also perform instant magic. Simply by typing __mkdir (make directory)__ plus a filename, presto! You have a new file in your current location. Like the most recent commands you learned, this can be done through _absolute_ or _relative_ paths.

It is just as simple to create files too. Simply type __touch__ and a filename (don't forget to add a type suffix!) and presto! You have a new file.

TBC....
