---
layout: post
title: Loading of materials
date: 2009-11-30 05:24
author: admin
comments: true
categories: [Uncategorized]
---
<a onblur="try {parent.deselectBloggerImageGracefully();} catch(e) {}" href="http://2.bp.blogspot.com/_LfYx03jjmdk/SxNn990tNRI/AAAAAAAAAuk/iBgMhD0nCTg/s1600/screen.jpg"><img class="image featured" src="http://2.bp.blogspot.com/_LfYx03jjmdk/SxNn990tNRI/AAAAAAAAAuk/iBgMhD0nCTg/s320/screen.jpg" border="0" alt="" id="BLOGGER_PHOTO_ID_5409781891667408146" /></a><br /> <br />  My previous demo had very long loading time (~4 min). There were many big textures there (usually 1024x1024), most of it in tga format.  <br />  To fix it, I changed format to dds, pack mips to texture and moved loading of textures to separate thread. Moreover, only near textures (~50 meters - engine parameter) are loaded and during moving, textures outside of that radius will be unloaded. Small versions of texture (64x64 usually) are used instead of full versions on a distance. <br />  Results - 3-4 sec for loading current outdoor level (~800 000 tris), unlimited number of  textures on a level, all in separate thread, important for today's multicore CPUs.
