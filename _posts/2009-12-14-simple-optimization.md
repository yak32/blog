---
layout: post
title: simple optimization
date: 2009-12-14 02:23
author: admin
comments: true
categories: [Uncategorized]
---
If you have vector assignment in your code, use Swap member function of std::vector, if you will not need source vector anymore it will save you one memory allocation

```C++
void SetPath_Dirty(vec3& path) {
	m_path.swap(path);
}
```
