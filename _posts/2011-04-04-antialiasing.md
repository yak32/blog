---
layout: post
title: Antialiasing
date: 2011-04-04 07:57
author: admin
comments: true
categories: [Uncategorized]
---
<p>Antialiasing is finally implemented in Glow engine.</p><p>It's implemented by <a href="http://and.intercon.ru/releases/talks/dlaagdc2011/">Directionally Localized AA algorithm</a>,implemented in The Force Unleashed 2. It's operates in image space and works as post-process, finding edges by High-Pass filter and blur it with 5x5 (and 16x16 for long edges) kernel.<br /></p><p>Looks cool .. my images long time suffered from jaggies .. not now)</p><p>Antialiasing is off:<br /><img border="3" alt="" src="http://2.bp.blogspot.com/-2gF7K-fMb2U/TZl6MGOC6kI/AAAAAAAABJg/IUy4Ax8Dofo/s320/aa_off.jpg" /><br /><p>Antialiasing is on:<br /><img border="3" alt="" src="http://3.bp.blogspot.com/-OAV5QGicLNw/TZl6Q9mA3lI/AAAAAAAABJo/zIIKs2_kBXw/s320/aa_on.jpg" /><br /></p>
