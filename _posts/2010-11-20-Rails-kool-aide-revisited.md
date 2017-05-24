---
layout: post
title: Drinking the Rails Kool-Aide, Revisited
categories: [Rails,software development]
---

A few years ago, I jotted down some thoughts about working with Rails in an Agile environment, under the somewhat provocative title I’ve used for this post. Here are some of those ideas. I’ve expanded on some, commented and clarified others. By no means an exhaustive list, here are some of the paradigms I’ve used when developing with Rails:

1. *Embrace change.* Forget how you did it before. Reproduce the results, not the methodology.
2. *Embrace design.* Accept that the two primary work areas for a development project are architecture and data modeling. 80% of your project effort should be in these areas. Not coding.
3. *Design from square one.* Don’t start by coding. Start with architecture. Model your database on a whiteboard. When you have the architecture where you think it should be, write tests. Coding too much too early will hamper success. If you can’t explain where you’re going, how can you know when you’ve arrived?
4. *Databases are for data.* If you have data to store, put it in the database. If you need data, get it out of the database. Flat files in the file system are almost never what you want in a web application.
5. *Understand the framework’s inherent biases.* For example, Rails doesn’t play well with certain concepts that are de rigueur in the database world, like domain keys, composite keys (although there’s a plugin for that), etc. There’s a longer post in this one, I think.
6. *Embrace DRY.* When you do code, embrace “don’t repeat yourself” and be draconian about it. Don’t program via cut-and-paste.
7. *Leverage the community*, or, to put it another way, *Don’t Repeat Others Either.* The initial thought when sitting down to code should be “where do I look for something already written that does what I want?” rather than “how am I going to do this?”
8. *Test everything.* Don’t ship code for which you haven’t written formal tests.
9. *Don’t optimize the framework away.* Optimization efforts should start with “How do I leverage the framework, given the overhead that I’ve paid already?” Worry about reducing the overhead only after you’ve gotten everything you can out of the framework.
