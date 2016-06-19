---
layout: post
title: Delete all branch except master
date: 2016-05-19 10:41:19.000000000 +05:45
type: post
published: true
status: publish
categories: []
tags: []

---

```
$ git branch | grep -v "master" | xargs git branch -D 
```

Instead of master if you can also delete other branch by replacing with any branch name

```
$ git branch | grep -v "<branch-name>" | xargs git branch -D 
```

