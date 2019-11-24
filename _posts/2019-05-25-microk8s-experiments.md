---
background: /assets/site/lake.jpg
layout: post
title: kubernetes experiments 
date: 2019-05-25 14:11 -0700
---

I've been playing around (learning) kubernetes, and decided to start a project that woud have some practical application. Unfortunately, most of the kubernetes tutorials that you find on the Internet fall into one of two categories:

+ those that focus on the infrastructure aspects, and hand you a pre-built container image that is largely opaque to you. 
+ those that focus on using stock container images, with external configuration. 

Because of how my brain works, I want something different. I want to 

+ Build a container image for an application that I'm familiar with
+ Create a pod that contains that application and the (stock) components that it requires. 

My project is a hubot deploymnet, with custom scripts, and a redis instance with persistent storage. 

In this series, I'm going to walk through how I created a container for alice, the hubot instance that supports a team that I'm a part of, and how I moved it from a local microk8s instance into a kubernetes cloud service. 
