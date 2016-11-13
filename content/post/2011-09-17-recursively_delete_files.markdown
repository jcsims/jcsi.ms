+++
categories = ["command line", "osx", "octopress"]
comments = false
date = "2011-09-17T00:00:00-07:00"
title = "Recursively deleting a file"
slug = "recursively-delete-files"
tags = []
+++

I ran into a small bug in the latest pull from the octopress source.  It was complaining about .DS_Store files:

	➜  jcsims.me git:(master) rake deploy
	rake aborted!
	No such file or directory - public/_layouts/.DS_Store

	Tasks: TOP => deploy
	(See full trace by running task with --trace)

It's currently an [issue][1], but in the short-term I needed to remove all the pesky files from the project.
Enter this nice and easy command (the `-delete` action is available in newer versions of `find`:

	find . -name ".DS_Store" -delete

[1]: https://github.com/imathis/octopress/issues/150
