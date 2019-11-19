---
layout: post
title: Editor features
date: 2010-08-25 05:02
author: admin
comments: true
categories: [engine]
youtubeId: N9XsXwIe9mQ
---
{% include youtubePlayer.html id=page.youtubeId %}


New features added to Glow engine editor during last  week. Previously, all level geometry was created in 3ds max and imported into game engine. It's not convenient (and not cheap) way of editing game level, so development of  Editor was started.<br /><br />After week it has next features - drag and drop meshes from Explorer (currently OBJ format, more later), simple Asset manager, executed as job (in parallel thread), so parsing 3d meshes will not stop UI.<br /><br />Also Undo/Redo is implemented ( with boost functors ). Currently it works for move/rotate/scale, delete/insert, select. Objects can be linked to landscape, so, for example, building and trees will be always on the ground. Rotation, movement will be in local or world coordinate system.<br /><br />Next things to implement: building level, attaching scripts to objects, assigning materials by drag and drop from Windows Explorer.
