---
layout: post
title: "Convert Bare Git Repository Into Normal Repository"
date: 2012-10-24 09:18
comments: true
categories: [git]
---

Suppose you have a bare Git repository and want to access and browse files in it. You can get a working copy like this:

For instance, your bare repository is `repo.git`.

* `mkdir repo`
* `cp repo.git repo/.git`
* `git config --bool core.bare false`
* `git checkout master`

You can know browse files and use regular git commands.
