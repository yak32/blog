---
layout: post
title: Mesh generation
subtitle: Greedy mesh generation for a voxel field
date: 2012-11-09 09:01
author: admin
comments: true
image: /blog/images/uploads/2012/11/screen_greedy_ambient_grid.jpg
categories: [Uncategorized]
---
I upgraded "greedy" mesh generation algorithm, mentioned <a href="http://glow3d.com/blog/2012/08/20/geometry-optimization/">here</a>  . Now it supports ambient lighting, prerendered into texture. As voxel world is cubic, we can just prerender all possible combination of ambient lighting on cube side into texture.

And with greedy mesh generation it will significantly improve rendering speed and physics updates. Voxels are sent to physics as mesh (actually same mesh, used for rendering, is sent to bullet physics).

<a href="/blog/images/uploads/2012/11/screen_greedy_ambient_grid.jpg"><img class="image featured" title="screen_greedy_ambient_grid" src="/blog/images/uploads/2012/11/screen_greedy_ambient.jpg" alt=""  /></a>

Previous, "dumb" mesh generation.
<a href="/blog/images/uploads/2012/11/screen_greedy_ambient_grid.jpg"><img class="image featured" title="screen_greedy_ambient_grid" src="/blog/images/uploads/2012/11/screen_grid.jpg" alt="" /></a>
