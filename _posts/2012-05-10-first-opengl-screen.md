---
layout: post
title: First OpenGL screen
date: 2012-05-10 02:25
author: yak32
comments: true
categories: [engine]
---
First screen of Tarta game, based on OpenGL renderer. Nothing special, but it's important for me - scheme, which I selected some time ago (some LONG ago) for cross platform development finally works.

![](/blog/images/uploads/2012/05/opengl_first_screen1.jpg){:class="img-responsive"}

Two weeks ago I tried compilation under GCC and Linux and finished it in 2-3 days without any significant problems.

Currently engine supports DirectX and OpenGL (primitively). OpenGL will allow me later to launch Glow engine on IOS and Android (plus Linux and MacOS)

Moreover, with usage of hlsl2glsl open source lib, it will be possible to use all sophisticated HLSL shaders from DirectX render automatically.
