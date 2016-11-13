+++
categories = ["mac", "osx", "terminal"]
comments = false
date = "2011-07-08T00:00:00-07:00"
title = "Unhide Library In Lion"
slug =  "unhide-library-in-lion"
tags = []
+++

For those of you who may have the benefit of already using Mac OSX Lion (or those of you who will be using it in the next two weeks), you may notice that the Library folder is now hidden in your home directory.  Luckily, there's an easy fix:

	chflags nohidden /Users/<Username>/Library

This was overwritten after upgrading between dev releases of Lion, so we may see this same issue continue in Lion.
