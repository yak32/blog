---
layout: post
title: Iron Cube 0.15
subtitle: Tank multiplayer combat in voxel world
date: 2013-07-03 07:31
author: admin
comments: true
categories: [game, iron cube]
---
<div class="videoWrapper"><iframe width="640" height="360" src="//www.youtube.com/embed/gOde2vm685M" frameborder="0" allowfullscreen></iframe></div>
<a style="line-height: 1.4;" title="Download Iron Cube 0.15 - Mod DB" href="http://www.moddb.com/games/iron-cube/downloads/iron-cube-015" target="_blank"><img alt="Iron Cube 0.15" src="http://button.moddb.com/download/medium/56386.png" /></a>

I spent several weeks on preparing Iron Cube release 0.15. Added a lot of new functionality, AI bots, dynamic navigation meshes, new voxel based lighting, new OpenGL based rendering and water.

AI Bots added to gameplay and they pretty smart! (not actually, same team member still can shoot each other, then one of them is on the line of fire, but it will be fixed soon). They can follow leader (player), find optimal way to enemy and give way to player. I am actually thinking how to make them slightly dumber.

Bots use new navigation system, based on updated Recast library. Meshes are dynamic, it means they will be rebuild, when voxels are changed.
<a href="/blog/images/uploads/2013/07/iron_cube_ai.jpg"><img class="image featured" alt="iron_cube_ai" src="/blog/images/uploads/2013/07/iron_cube_ai.jpg"/></a>

And demonstration, how dynamic navigation meshes work
<div class="videoWrapper"><iframe src="//www.youtube.com/embed/I1bS-wjuFks?rel=0" height="480" width="640" allowfullscreen="" frameborder="0"></iframe></div>
New voxel-based lighting system is developed, lighting from sun is ambient and allows smooth shadows (relatively smooth, because of overall pixelated style). Lighting made using modified flood-fill of skylight from top of the world.
<a href="/blog/images/uploads/2013/07/iron_cube_lighting.jpg"><img class="image featured" alt="iron_cube_lighting" src="/blog/images/uploads/2013/07/iron_cube_lighting.jpg"/></a>

Also I switched render from DirectX+Deferred Shading to OpenGL+simple voxel based lighting, to be compatible with future mobile ports. It's faster and allows to play game on old hardware.

A lot of work made in editor, it's now fully functional, allows to render random polygonal models into voxel world, edit mesh, setup lighting and AI.

One step closer to final release!
