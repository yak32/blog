---
layout: post
title: Iron Cube 0.15
subtitle: Tank multiplayer combat in a voxel world
date: 2013-07-03 07:31
author: admin
comments: true
categories: [game, iron cube]
youtubeId: gOde2vm685M
---
{% include youtubePlayer.html id=page.youtubeId %}

<a style="line-height: 1.4;" title="Download Iron Cube 0.15 - Mod DB" href="http://www.moddb.com/games/iron-cube/downloads/iron-cube-015" target="_blank"><img alt="Iron Cube 0.15" src="http://button.moddb.com/download/medium/56386.png" /></a>

I spent several weeks on preparing the Iron Cube release (v.0.15.). I added a lot of new functionalities, AI bots, dynamic navigation meshes, new voxel based lighting and new OpenGL based rendering and water.

AI Bots are added to gameplay, and they're pretty smart! (actually not really, a team member still can shoot one of its own friends when one of them is on the line of fire, but it will be fixed soon). They can follow their leader (player), find an optimal way to find the enemy and give way to the player. I am actually thinking how to make them slightly dumber.

Bots use new navigation systems, based on the updated Recast library. Meshes are dynamic, it means they will be rebuilt when the voxels are changed.
![](/blog/images/uploads/2013/07/iron_cube_ai.jpg){:class="img-responsive"}

And now a demonstration on how dynamic navigation meshes work:

{% include youtubePlayer.html id="I1bS-wjuFks" %}
a new voxel-based lighting system is developed, the lighting from the sun is ambient and allows smooth shadows (relatively smooth, because of the overall pixelated style). Lighting is made using a modified flood-fill of skylight from the top of the world.
![](/blog/images/uploads/2013/07/iron_cube_lighting.jpg){:class="img-responsive"}

Also I switched the render from DirectX+Deferred Shading to an OpenGL+simple voxel based lighting to be compatible with future mobile ports. It's faster and allows you to play the game on old hardware.

A lot of work was put into making the editor, and it's now fully functional, allowing you to render random polygonal models into the voxel world, edit the meshes, setup lighting and AI.

Now I'm one step closer to the final release!
