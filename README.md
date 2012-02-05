What is this?
========

Window Tools is a collection of scripts for manipulating windows on various Linux desktop environments.  The general purpose of these tools is to augment window switching across multiple virtual desktops in a way that doesn't obfuscate your focus, involve clicking around with the mouse, or using Gnome 3/Unity.  Ideally, you should be able to bind them to a keyboard shortcut and have then behave as ubiquitously as existing Compiz or X Window functionality.

Installation
========

First, you'll need to install the excellent X Window Manager control tool known as **wmctrl**.  On a recent version of Ubuntu, try something like this:

    sudo apt-get install wmctrl

Also, if you don't already have it, go grab **zenity** for prompting users with all kinds of text boxes:

    sudo apt-get install zenity

Next, find a script that you like and copy it over to some place on your default path, as in:

    sudo cp ./bin/windowtool /usr/local/bin

Current Tools
========

*windowtool [list]*

Running **windowtool** with no parameters will prompt you to search for a window by its name (window title).  This uses the default window title matching algorithm from **wmctrl**. Passing the *list* parameter will also print out all the current window titles of all open windows on all desktops. SUPER+SPACE seems to be a reasonable binding if you're not using it.

