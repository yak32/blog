---
layout: post
title: First horde tests
date: 2009-12-24 10:36
author: admin
comments: true
categories: [Uncategorized]
---
Spent day for implementing steering behaviors for horde. <br /> <br />Recast navigation + avoid nearest neighbor (with prediction, OpenSteer style) + avoid near walls<br /><br /><object width="425" height="344"><param name="movie" value="http://www.youtube.com/v/uH4lo1gW2K8&amp;hl=en_US&amp;fs=1&amp;"><param name="allowFullScreen" value="true"><param name="allowscriptaccess" value="always"><embed src="http://www.youtube.com/v/uH4lo1gW2K8&amp;hl=en_US&amp;fs=1&amp;" type="application/x-shockwave-flash" allowscriptaccess="always" allowfullscreen="true" width="425" height="344"></embed></object><br /><br />Recast navigation + avoid nearest neighbor (with prediction, OpenSteer style) + avoid walls only after collision + avoid dynamic obstacles <br />  <object width="425" height="344"><param name="movie" value="http://www.youtube.com/v/_gStLaNyJ24&amp;hl=en_US&amp;fs=1&amp;"><param name="allowFullScreen" value="true"><param name="allowscriptaccess" value="always"><embed src="http://www.youtube.com/v/_gStLaNyJ24&amp;hl=en_US&amp;fs=1&amp;" type="application/x-shockwave-flash" allowscriptaccess="always" allowfullscreen="true" width="425" height="344"></embed></object> <br />  It needs time to update nav mesh (usually nav mesh updated with 0.5 sec intervals), so sometimes bots can go throw obstacle. Maybe for moving obstacles I need to use same steering behavior as for another bots.  <br />  Does it look natural? Or need some enhancements?
