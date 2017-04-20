---
layout: post
title: Normal texture trick
date: 2010-12-01 12:58
author: admin
comments: true
categories: [Uncategorized]
---
I found interesting trick  for accessing normals from textures. <br />  <a href="http://code.google.com/p/nvidia-texture-tools/wiki/NormalMapCompression">http://code.google.com/p/nvidia-texture-tools/wiki/NormalMapCompression</a></span></h3></span> <br />  Shortly, it allows to use DXT1 and DXT5 bump textures with same shaders.   It's important for editor because  bump texture in DXT5 will be ready only  at the last stage -   game packaging. There will be small difference in object appearance during in-Editor testing because DXT1 is not good for normals, but I think it's acceptable.
