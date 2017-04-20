---
layout: post
title: First screen of voxel field update by network.
date: 2012-05-25 00:09
author: yak32
comments: true
categories: [Uncategorized]
---
Cool,  today I implemented update of voxel field in multiplayer environment.
Currently update of voxels is sent per chunk of voxels (32x32x64) and compressed by RLE.
Implemented using UDP networking, as other client-server communication. Update of voxel field is done
on server and sent to client.

<a href="/images/uploads/2012/05/tarta_net_hole2.jpg"><img class="alignnone size-full wp-image-183" title="tarta_net_hole" src="/images/uploads/2012/05/tarta_net_hole2.jpg" alt="" width="655" height="517" /></a>
