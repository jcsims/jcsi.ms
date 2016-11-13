+++
categories = ["git"]
comments = false
draft = false
date = "2011-05-29T00:00:00-07:00"
title = "Delete A Remote Git Branch"
slug = "delete-a-remote-git-branch"
tags = []
+++

A quick note on how to remove a remote git branch.  When using [git flow](http://nvie.com/posts/a-successful-git-branching-model/)
(which I highly recommend), I've found myself with remote branches pushed to github, but removed locally, for example after a
feature has been completed.  This is a quick one-liner to remove a target remote branch:

	git push REMOTENAME :BRANCHNAME

This is explained [here](http://help.github.com/remotes/) on github's help.
