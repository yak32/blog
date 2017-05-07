---
layout: post
title: Zelda-like game.
subtitle: The game prototype without title.
date: 2017-05-07 23:13
author: admin
comments: true
categories: [game]
---
<div class="videoWrapper"><iframe width="560" height="315" src="https://www.youtube.com/embed/dsCfWE7WE1c" frameborder="0" allowfullscreen></iframe></div>

A youtube video from the voxel [game prototype]({{ site.url }}{{ site.baseurl }}/engine/games/2017/04/20/voxel-project.html) I built on my **Glow3D** engine some time ago. The idea was something like original Zelda game (isometric, adventure, but on voxels). Art from the video was created by [Sir carma](https://twitter.com/sir_carma?lang=en). I built a parser of the MagicaVoxel file format and updated significantly the source code I created for [Iron Cube game]({{ site.url }}{{ site.baseurl }}/game/iron%20cube/2013/10/23/iron-cube-tank-multiplayer-combat-in-voxel-world-is-ported-to-android-and-available-on-google-play-store-for-free.html). Support for nVidia HBAO+ and nVidia Shadows was added using [Shadow Works middleware](https://developer.nvidia.com/shadowworks) to improve picture quality. nVidia HBAO+ is *Screen space ambient occlusion* technology to emulate global illumination and I give up to create my own implementation of SSAO (at least for some time). I have support for shadows in the engine but didn't have efficient Cascaded Shadow Maps at that time and decided to use nVidia libraries for it. It's efficient and used in many modern games.

[MagicaVoxel]([Magica](https://ephtracy.github.io/)) is a nice voxel editor and renderer, created by [@ephtracy](https://twitter.com/ephtracy?lang=en). He basically did 3D Studio Max alone but only for voxel graphics. Sound used for the video is [Medieval Introduction](http://www.freesound.org/people/Tristan_Lohengrin/sounds/319781/).





