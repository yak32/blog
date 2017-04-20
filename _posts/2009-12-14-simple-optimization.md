---
layout: post
title: simple optimization
date: 2009-12-14 02:23
author: admin
comments: true
categories: [Uncategorized]
---
If you have vector assignment in your code, <br />use Swap member function of std::vector, if<br />you will not need source vector anymore<br /><br />it will save you one memory allocation<br /><br />void SetPath_Dirty(vec3& path)<br />{<br />    m_path.swap(path);<br />}
