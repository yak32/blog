---
layout: post
title: Project Mercury
subtitle: Project Mercury - 3d mesh editor with bare hands
date: 2013-02-22 09:32
author: admin
comments: true
categories: [Mercury, prototype]
youtubeId: y6779QOnh6A
---
I participated in the Intel Perceptual Computing Challenge with project Mercury, Digital Sculpting Application - voxel-based 3D mesh edition with bare hands.

{% include youtubePlayer.html id=page.youtubeId %}

The prototype is based on the Glow engine and uses a voxel engine, which was made for the <a href="http://www.moddb.com/games/iron-cube">Iron Cube</a> game. Smooth mesh generation was additionally written, which is based on Surface Nets (like modification of Matching Cubes)

<a href="http://software.intel.com/en-us/vcsource/tools/perceptual-computing-sdk">The Intel Perceptual Computing SDK</a> and the <strong><a href="http://click.intel.com/intelsdk/Creative_Interactive_Gesture_Camera_Developer_Kit-P2061.aspx">Creative* Interactive Gesture Camera Developer Kit</a></strong> are used for hand-based interface. I received a camera just one day before mydeadline, so I had only one day to integrate it to the engine. And surprisingly it was done just in a few hours - SDK has a special util library, which makes it easy to use the camera's features.

SDK reports about several types of commonly used gestures like victory (V), "Thumbs signal" etc and reports about exact 3D positions of every finger. Also it reports about the hand state (open, close) and position.

Only restricted gestures and manipulations are supported currently in the Mercury project, but I hope to make it as easy as in real sculpting. The camera provides enough precision to make it.
