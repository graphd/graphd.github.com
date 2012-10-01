---
layout: post
title: "Git in color"
date: 2012-10-01 10:46
comments: true
categories: [git, visualization]
---

This will add colors on git-diff, git-log, git-*:

    git config --global --add color.ui true

* `git-diff` will color changes you have made.
* `git-log` will color commit hashed yellow.
* `git-branch` will color your current branch green and remote branches red.
* `git-status` will color files in your index green. New and changed files are red.
