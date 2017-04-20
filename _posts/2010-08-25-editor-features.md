---
layout: post
title: Editor features
date: 2010-08-25 05:02
author: admin
comments: true
categories: [Uncategorized]
---
<object width="425" height="344"><param name="movie" value="http://www.youtube.com/v/N9XsXwIe9mQ?fs=1&amp;hl=en_US"><param name="allowFullScreen" value="true"><param name="allowscriptaccess" value="always"><embed src="http://www.youtube.com/v/N9XsXwIe9mQ?fs=1&amp;hl=en_US" type="application/x-shockwave-flash" allowscriptaccess="always" allowfullscreen="true" width="425" height="344"></embed></object><br /><br />New features added to Glow engine editor during last  week. Previously, all level geometry was created in 3ds max and imported into game engine. It's not convenient (and not cheap) way of editing game level, so development of  Editor was started.<br /><br />After week it has next features - drag and drop meshes from Explorer (currently OBJ format, more later), simple Asset manager, executed as job (in parallel thread), so parsing 3d meshes will not stop UI.<br /><br />Also Undo/Redo is implemented ( with boost functors ). Currently it works for move/rotate/scale, delete/insert, select. Objects can be linked to landscape, so, for example, building and trees will be always on the ground. Rotation, movement will be in local or world coordinate system.<br /><br />Next things to implement: building level, attaching scripts to objects, assigning materials by drag and drop from Windows Explorer.
