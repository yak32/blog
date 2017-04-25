---
layout: post
title: Voxelization
date: 2012-10-23 17:46
author: admin
comments: true
categories: [game, iron cube, voxel]
---
I played with automatic voxelization of 3d model.

Original model: <a href="/blog/images/uploads/2012/10/tank_original.jpg"><img class="image featured" title="tank_original" src="/blog/images/uploads/2012/10/tank_original.jpg" alt=""/></a>

&nbsp;

Model after voxelization:
<a href="/blog/images/uploads/2012/10/tank_voxelized.jpg"><img class="image featured" title="tank_voxelized" src="/blog/images/uploads/2012/10/tank_voxelized.jpg" alt=""/></a>

Model was voxelized into 50x50x50 voxel field so resolution should be definitely increased. Model is rasterized into voxel field polygon by polygon similarly to scan line 2d algorithm.
