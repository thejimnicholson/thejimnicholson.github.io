---
layout: post
title: List Makefile targets
categories: [unix,linux,bash,shell]
background: /assets/site/lake.jpg
---

This snippet can be helpful if you frequently work with large Makefiles. 

```
make -qp | awk -F':' '/^[a-zA-Z0-9][^$#\/\t=]*:([^=]|$)/ {split($1,A,/ /);for(i in A)print A[i]}'
```
