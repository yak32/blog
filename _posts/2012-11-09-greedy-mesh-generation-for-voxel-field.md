---
layout: post
title: Greedy mesh generation for voxel field
date: 2012-11-09 09:01
author: admin
comments: true
categories: [Uncategorized]
---
I upgraded "greedy" mesh generation algorithm, mentioned <a href="http://glow3d.com/blog/2012/08/20/geometry-optimization/">here</a>  . Now it supports ambient lighting, prerendered into texture. As voxel world is cubic, we can just prerender all possible combination of ambient lighting on cube side into texture.

And with greedy mesh generation it will significantly improve rendering speed and physics updates. Voxels are sent to physics as mesh (actually same mesh, used for rendering, is sent to bullet physics).

<a href="/images/uploads/2012/11/screen_greedy_ambient_grid.jpg"><img class="alignnone size-full wp-image-339" title="screen_greedy_ambient_grid" src="/images/uploads/2012/11/screen_greedy_ambient_grid.jpg" alt="" width="668" height="522" /></a>

<a href="/images/uploads/2012/11/screen_greedy_ambient_grid.jpg"><img class="alignnone size-full wp-image-339" title="screen_greedy_ambient_grid" src="/images/uploads/2012/11/screen_greedy_ambient.jpg" alt="" width="668" height="522" /></a>

Previous, "dumb" mesh generation.
<a href="/images/uploads/2012/11/screen_greedy_ambient_grid.jpg"><img class="alignnone size-full wp-image-339" title="screen_greedy_ambient_grid" src="/images/uploads/2012/11/screen_grid.jpg" alt="" width="668" height="522" /></a>
