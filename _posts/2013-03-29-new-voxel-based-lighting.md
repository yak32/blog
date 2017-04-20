---
layout: post
title: New voxel based lighting
date: 2013-03-29 12:18
author: admin
comments: true
categories: [Uncategorized]
---
<a href="/blog/images/uploads/2013/03/iron_cube_lighting.jpg"><img class="alignnone size-full wp-image-444" alt="iron_cube_lighting" src="/blog/images/uploads/2013/03/iron_cube_lighting.jpg" width="700" height="543" /></a>
I implemented new CPU based lighting, which will helps with rendering on mobile devices. Lighting divided into sky and local lighting. Sky emits lights from top to bottom of voxel world, it creates shadows and darken caves. Local lights currently without shadows but uses normals of objects. Lights are calculated in editor and saved to file to help with load time on mobile devices.
