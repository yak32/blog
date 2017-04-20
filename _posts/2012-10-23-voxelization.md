---
layout: post
title: Voxelization
date: 2012-10-23 17:46
author: admin
comments: true
categories: [Uncategorized]
---
I played with automatic voxelization of 3d model.

Original model: <a href="/images/uploads/2012/10/tank_original.jpg"><img class="alignnone  wp-image-324" title="tank_original" src="/images/uploads/2012/10/tank_original.jpg" alt="" width="700" /></a>

&nbsp;

Model after voxelization:
<a href="/images/uploads/2012/10/tank_voxelized.jpg"><img class="alignnone size-full wp-image-325" title="tank_voxelized" src="/images/uploads/2012/10/tank_voxelized.jpg" alt="" width="700" /></a>

Model was voxelized into 50x50x50 voxel field so resolution should be definitely increased. Model is rasterized into voxel field polygon by polygon similarly to scan line 2d algorithm.
