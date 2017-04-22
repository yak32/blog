---
layout: post
title: Quternion trick
date: 2010-08-05 06:53
author: admin
comments: true
categories: [Uncategorized]
---
Long time ago i wrote function, which creates quaternion for rotation from 0,0,1 to any unit vector. Function was very long, contained asin, acos, several conditions etc... So today i returned and after some time: dir should be unit

```C++
void Quaternion::from_direction(const vec3 dir){
	x = dir.y;
	y = -dir.x;  z = 0;
	w = 1 + dir.z; // simplified dot product with 0,0,1
	normalize();
}
```
