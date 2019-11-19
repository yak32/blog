---
layout: post
title: Voxelization
date: 2012-10-23 17:46
author: admin
comments: true
categories: [game, iron cube, voxel]
---
I played with automatic voxelization of 3d model.

Original model: 
![](/blog/images/uploads/2012/10/tank_original.jpg){:class="img-responsive"}

&nbsp;

Model after voxelization:
![](/blog/images/uploads/2012/10/tank_voxelized.jpg){:class="img-responsive"}

Model was voxelized into 50x50x50 voxel field so resolution should be definitely increased. Model is rasterized into voxel field polygon by polygon similarly to scan line 2d algorithm.
