---
layout: post
title: Disable gnome screensaver from command line
categories: [unix,linux,gnome ]
---

Works for gnome 2.

```
gconftool-2 --set /apps/gnome-power-manager/timeout/sleep_display_ac 0 --type int
gconftool-2 --set /apps/gnome-screensaver/lock_enabled false --type bool
gconftool-2 --set /apps/gnome-screensaver/idle_activation_enabled  false --type bool
```
