---
layout: post
title: First horde tests
date: 2009-12-24 10:36
author: admin
comments: true
categories: [engine, ai]
youtubeId: uH4lo1gW2K8
---
Spent day for implementing steering behaviors for horde. <br /> <br />Recast navigation + avoid nearest neighbor (with prediction, OpenSteer style) + avoid near walls

Recast navigation + avoid nearest neighbor (with prediction, OpenSteer style) + avoid walls only after collision + avoid dynamic obstacles

{% include youtubePlayer.html id="_gStLaNyJ24" %}



It needs time to update nav mesh (usually nav mesh updated with 0.5 sec intervals), so sometimes bots can go throw obstacle. Maybe for moving obstacles I need to use same steering behavior as for another bots. Does it look natural? Or need some enhancements?
