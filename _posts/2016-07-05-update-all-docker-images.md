---
layout: post
title: Update all docker images
date: 2016-07-15 10:41:19.000000000 +05:45
type: post
published: true
status: publish
categories: []
tags: []

---

```
$ docker images | awk '{print $1}' | xargs -L1 docker pull
```

