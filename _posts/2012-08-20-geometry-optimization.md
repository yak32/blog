---
layout: post
title: Geometry optimization
date: 2012-08-20 13:04
author: admin
comments: true
categories: [Uncategorized]
---
I applied some optimization to the mesh generation. Previously, voxel mesh was generated as-is, with removing only internal faces. It creates huge amount of vertex data, which was slowly loaded into gpu, slowly processed on cpu etc. New algorithm reduce vertex data in 3-4 times, but slightly increase time of mesh generation. Also, one possible minus of new algorithm - it will be hard to apply ambient occlusion, based on vertexes (it's not regular mesh now), but I hope my version of SSAO will handle it.
<a href="/blog/images/uploads/2012/08/screen_detail1.jpg"><img class="image featured" title="screen_detail" src="/blog/images/uploads/2012/08/screen_detail1.jpg" alt=""/></a>

It's new version of mesh generation.
<img class="image featured" title="tarta_greedy" src="/blog/images/uploads/2012/08/tarta_greedy1.jpg" alt="" />/>;
