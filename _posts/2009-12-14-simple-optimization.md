---
layout: post
title: simple optimization
date: 2009-12-14 02:23
author: admin
comments: true
categories: [engine, C++]
---
If you have vector assignment in your code, use Swap member function of std::vector, if you will not need source vector anymore it will save you one memory allocation

```cpp
void SetPath_Dirty(vec3& path) {
	m_path.swap(path);
}
```
