---
layout: post
title: Simple steering behavior
date: 2009-12-15 08:23
author: admin
comments: true
categories: [engine, ai]
---
I added yesterday simple steering behavior for bots. Movement became more realistic than previous direct path following. Now bot has  velocity and acceleration, and it tries to move along current path line.

<div class="videoWrapper"><object width="425" height="344"><param name="movie" value="//www.youtube.com/v/Pw7GRTxxnYA&hl=en_US&fs=1&"></param><param name="allowFullScreen" value="true"></param><param name="allowscriptaccess" value="always"></param><embed src="//www.youtube.com/v/Pw7GRTxxnYA&hl=en_US&fs=1&" type="application/x-shockwave-flash" allowscriptaccess="always" allowfullscreen="true" width="425" height="344"></embed></object></div>

  Remaining task - dealing with walls (current bot position now not exactly on the safe path), moving obstacles.
