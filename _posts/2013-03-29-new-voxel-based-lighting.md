---
layout: post
title: Lighting
subtitle: New voxel based lighting
date: 2013-03-29 12:18
author: admin
comments: true
image: /blog/images/uploads/2013/03/iron_cube_lighting.jpg
categories: [game, iron cube]
---
I implemented the new CPU based lighting, which helps with rendering on mobile devices. Lighting is divided into sky and local lighting. Sky emits lights from top to bottom of the voxel world, also it creates shadows and darkens caves. Local light's currently without shadows, but uses normals of objects. Lights are calculated in the editor and then saved to the file to help with loading time on mobile devices.
