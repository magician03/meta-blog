+++
title = "Solarized-Dark theme configuration in Terminator"
description = ""
tags = [
    "linux",
]
date = "2017-01-14"
categories = [
    "Linux",
]
menu = "main"
+++


#### Intro

Terminator is an open-source terminal emulator project with an aim to produce a
useful tool for arranging terminals. You can split a window into many tabs and
tabs into child terminals.

#### Configuration

To configure your termiantor theme to solarised-dark, you need to modify the
file located at `~/.config/terminator/config` in your linux system.

Here is a preview of what it looks like when done:

{{< figure src="https://cdn-images-1.medium.com/max/900/1*lhwAer0NOlQTaveQytiwzA.png" caption="" >}}

Now to get this theme, replace the contents of `~/.config/terminator/config` file with the following:

{{< gist magician03 bd902770b3ccff82dd54fd5c361381a4 >}}

That’s it. You’re done ! Restart your terminal and enjoy the new theme.

You can also add various key-bindings by right-clicking anywhere, then
Perferences>KeyBindings.

You change modify the settings as per your desires and needs simply by editing
the attributes of default theme mentioned in config file.

Comment below for any queries or suggestions.

[Here](https://medium.com/@magician03/solarized-dark-theme-configuration-in-terminator-4b106d0b0c58) is the Medium article for this post.