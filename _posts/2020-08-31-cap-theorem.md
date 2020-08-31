---
layout: post
title:  "CAP Theorem"
date:   2020-08-31 20:22:36 +0530
categories: jekyll update
---

# CAP THEOREM
### What is CAP Theorem ?
CAP stands for :
> __C__ -> *Consistency*
> __A__ -> *Availability*
> __P__ -> *Partition tolerance*

It states that it is impossible for a distributed system to hold all the three properties at the same time, i.e, for a distributed system , atmost it is guarantees to hold two out of three properties.

Lets move forward in other to understand what each word means and will also see scenarios which will prove the above said statement.

__Consistency__ **:** For multiple read request, we should always get same values or an error. Lets take a scenario that we have a node which has multiple replicas , so in this case consistency can only be achived if we allow read operation after all the nodes have latest value after each write operation

__Availability__ **:** Every request made to a non-failing server in a distributed system must result in a response. In short, request should never be ignored by the servers untill and unless that server to which the request has been routed is down. 

__Partition tolerance__ **:** System continues to function even if these is communication failure between the node. In Distributed System we have multiple copies or in betters word, replicas of data and servers which help is running the system even after network failure between the nodes untill the whole network is not down.

> __Proof of CAP theorem :__

