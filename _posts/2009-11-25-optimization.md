---
layout: post
title: Optimization
date: 2009-11-25 10:17
author: admin
comments: true
categories: [Uncategorized]
---
 During tests, my game has average 40 fps on GeForce 9600 with Intel quad  core CPU.  That version was sent to IGF.   <br />  Several days ago I found, that  all shadows on level are drawn every frame. After searching in source I found commented for debugging line of code, which increase speed twice!  So fps becomes ~ 80. After switching off grass and NPC sensor system  (which do search for enemies 5 times per second) fps becomes 400!.  <br />  So first of all I implemented correct instancing for a grass ( and cut off all cards without support of Shader model 3).  Next step - faster sensor system for nps.  <br />  Now average fps is 160 but there are a lot of ways for improvement.
