---
layout: post
title: The Challenge
subtitle: Intel Perceptual Computing Challenge, stage 2
date: 2013-11-12 05:49
author: admin
comments: true
categories: [voxel, Intel, challenge]
---
<div class="videoWrapper"><iframe src="//www.youtube.com/embed/EzSByIMRiJk?rel=0&amp;wmode=opaque" height="480" width="640" frameborder="0"></iframe></div>
I participated in Intel Perceptual Computing Challenge, stage 2, improved my first prototype, which <a href="http://glow3d.com/blog/2013/03/28/first-prize-winner-of-intel-perceptual-computing-challenge/">won</a> First Prize of 1st stage. Intel SDK was improved since June, became more robust. Last time I received camera just before one day before deadline, so didn't have enough time to properly implement gesture support.

In current demo, I added several new gestures - size of brush can be changed by "zoom" gesture (moving open hands), undo of previous operation is implemented by "circle" gesture, provided by SDK, start of "potter" mode by swipe gesture (up, down, left, right). Also API was changed from DirectX to OpenGL, lighting became more simpler (forward) to optimize rendering. Save/Load of model was added. There are many improvements with robustness and smoothness of brush movement there.

It's became some kind of Paint editor for voxel models.

&nbsp;
