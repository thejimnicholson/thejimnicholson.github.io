---
layout: post
title: Display percent of disk space used on volume
categories: [unix,linux,bash,shell]
background: /assets/site/lake.jpg
---

Useful for writing monitor scripts, creating trigger events based on percentage, etc.
```
df / --total -x tmpfs | tail -1 | awk '{ print $5 }'
```
