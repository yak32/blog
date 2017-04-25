---
layout: post
title: Color transformations
date: 2011-04-04 08:40
author: admin
comments: true
categories: [engine]
---
Color transformations as Post-Process is added into Glow engine.

Currently supported transformations are contrast, brightness, black and white, red, green, blue shifts, saturation will be added later. All transformations work in a same step, so adding, for example contrast to brightness will not slow down it in 2 times.

Transformations added as scene property, and can be accessed from script.

Image:
<a onblur="try {parent.deselectBloggerImageGracefully();} catch(e) {}" href="http://1.bp.blogspot.com/-KCVm4VcaR44/TZmFs58S2AI/AAAAAAAABJw/zDuQV2MvVLA/s1600/cc_step1.jpg"><img id="BLOGGER_PHOTO_ID_5591647418871633922" class="image featured" src="http://1.bp.blogspot.com/-KCVm4VcaR44/TZmFs58S2AI/AAAAAAAABJw/zDuQV2MvVLA/s1600/cc_step1.jpg" alt="" border="0" /></a>

Adjusted brightness:
<a onblur="try {parent.deselectBloggerImageGracefully();} catch(e) {}" href="http://1.bp.blogspot.com/-DdRftU6v1sc/TZmFzZLUBXI/AAAAAAAABJ4/47bXJWtm2tE/s1600/cc_step2.jpg"><img id="BLOGGER_PHOTO_ID_5591647530335339890" class="image featured" src="http://1.bp.blogspot.com/-DdRftU6v1sc/TZmFzZLUBXI/AAAAAAAABJ4/47bXJWtm2tE/s1600/cc_step2.jpg" alt="" border="0" /></a>

Blue and Green shifted, to create Matrix movie look
<a onblur="try {parent.deselectBloggerImageGracefully();} catch(e) {}" href="http://2.bp.blogspot.com/-9gxCDszrOBo/TZmF5nMgwHI/AAAAAAAABKA/4jwt5VAPL1M/s1600/cc_step3.jpg"><img id="BLOGGER_PHOTO_ID_5591647637177679986" class="image featured" src="http://2.bp.blogspot.com/-9gxCDszrOBo/TZmF5nMgwHI/AAAAAAAABKA/4jwt5VAPL1M/s1600/cc_step3.jpg" alt=""border="0" /></a>

Black and white:
<a onblur="try {parent.deselectBloggerImageGracefully();} catch(e) {}" href="http://1.bp.blogspot.com/-viSCRwKufwA/TZmF9B_5UvI/AAAAAAAABKI/57miUou09mE/s1600/cc_step4.jpg"><img id="BLOGGER_PHOTO_ID_5591647695912129266" class="image featured" src="http://1.bp.blogspot.com/-viSCRwKufwA/TZmF9B_5UvI/AAAAAAAABKI/57miUou09mE/s1600/cc_step4.jpg" alt=""border="0" /></a>
