---
layout: post
title: The Challenge
subtitle: Intel Perceptual Computing Challenge, stage 2
date: 2013-11-12 05:49
author: admin
comments: true
categories: [voxel, Intel, challenge]
youtubeId: EzSByIMRiJk
---

{% include youtubePlayer.html id=page.youtubeId %}

I participated in the Intel Perceptual Computing Challenge, stage 2, where I improved my first prototype, which <a href="http://glow3d.com/blog/challenge/intel/winner/2013/03/28/first-prize-winner-of-intel-perceptual-computing-challenge.html">won</a> a First Prize of a 1st stage. Intel SDK was improved since June, becoming more robust. Last time I received a camera one day before my deadline, so didn't have enough time to properly implement gesture support.

In the current demo, I added several new gestures - the size of brush can be changed by a "zoom" gesture (moving open hands), undo of previous operation is implemented by a "circle" gesture, provided by SDK, start of "potter" mode by swiping up, down, left, or right. Also API was changed from DirectX to OpenGL and lighting became more simpler (forward) to optimize rendering. Save/Load of the model was added. There are many improvements with robustness and smoothness of brush movement there.

It has now become some kind of Paint editor for voxel models.

&nbsp;
