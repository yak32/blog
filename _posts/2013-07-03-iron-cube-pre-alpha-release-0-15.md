---
layout: post
title: Iron Cube 0.15
subtitle: Tank multiplayer combat in a voxel world
date: 2013-07-03 07:31
author: admin
comments: true
categories: [game, iron cube]
---
<div class="videoWrapper"><iframe width="640" height="360" src="//www.youtube.com/embed/gOde2vm685M" frameborder="0" allowfullscreen></iframe></div>
<a style="line-height: 1.4;" title="Download Iron Cube 0.15 - Mod DB" href="http://www.moddb.com/games/iron-cube/downloads/iron-cube-015" target="_blank"><img alt="Iron Cube 0.15" src="http://button.moddb.com/download/medium/56386.png" /></a>

I spent several weeks on preparing the Iron Cube release (v.0.15.). I added a lot of new functionalities, AI bots, dynamic navigation meshes, new voxel based lighting and new OpenGL based rendering and water.

AI Bots are added to gameplay, and they're pretty smart! (actually not really, a team member still can shoot one of its own friends when one of them is on the line of fire, but it will be fixed soon). They can follow their leader (player), find an optimal way to find the enemy and give way to the player. I am actually thinking how to make them slightly dumber.

Bots use new navigation systems, based on the updated Recast library. Meshes are dynamic, it means they will be rebuilt when the voxels are changed.
<a href="/blog/images/uploads/2013/07/iron_cube_ai.jpg"><img class="image featured" alt="iron_cube_ai" src="/blog/images/uploads/2013/07/iron_cube_ai.jpg"/></a>

And now a demonstration on how dynamic navigation meshes work:
<div class="videoWrapper"><iframe src="//www.youtube.com/embed/I1bS-wjuFks?rel=0" height="480" width="640" allowfullscreen="" frameborder="0"></iframe></div>
a new voxel-based lighting system is developed, the lighting from the sun is ambient and allows smooth shadows (relatively smooth, because of the overall pixelated style). Lighting is made using a modified flood-fill of skylight from the top of the world.
<a href="/blog/images/uploads/2013/07/iron_cube_lighting.jpg"><img class="image featured" alt="iron_cube_lighting" src="/blog/images/uploads/2013/07/iron_cube_lighting.jpg"/></a>

Also I switched the render from DirectX+Deferred Shading to an OpenGL+simple voxel based lighting to be compatible with future mobile ports. It's faster and allows you to play the game on old hardware.

A lot of work was put into making the editor, and it's now fully functional, allowing you to render random polygonal models into the voxel world, edit the meshes, setup lighting and AI.

Now I'm one step closer to the final release!
