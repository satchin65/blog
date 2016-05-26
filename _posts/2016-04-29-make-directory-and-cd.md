---
layout: post
title: Make directory & cd into (efficient method)
date: 2016-04-29 19:41:19.000000000 +05:45
type: post
published: true
status: publish
categories: []
tags: []

---
One the most common task you might do is something like:-

```
$ mkdir some/directory && cd some/directory
```

There is a clear problem of typing new directory name twice and sometime there can be some typo and we all have typing. So the most efficient way for doing this is:-

```
$ mkdir some/directory && cd $_
```
