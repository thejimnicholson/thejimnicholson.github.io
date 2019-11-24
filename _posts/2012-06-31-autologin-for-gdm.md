---
layout: post
title: Disable gnome screensaver from command line
categories: [unix,linux,gnome ]
background: /assets/site/lake.jpg
---

Edit /etc/gdm/custom.conf to add the following two lines in the daemon section:

```
[daemon]
AutomaticLoginEnable=True
AutomaticLogin=username
```
