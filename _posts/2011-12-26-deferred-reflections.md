---
layout: post
title: Deferred reflections
date: 2011-12-26 02:04
author: yak32
comments: true
categories: [Uncategorized]
---
<a href="/blog/images/uploads/2011/12/glow_deferred_reflections.jpg"><img class="image featured" title="glow_deferred_reflections" src="/blog/images/uploads/2011/12/glow_deferred_reflections.jpg" alt="Deferred reflections in Glow engine" /></a>

I thought about it a lot - how to implement planar reflection in engine with deferred lighting? Render scene with lighting (and shadows) into separate render target is very expensive - it doubles all calculations. And after I met idea about deferred reflections in article about rendering technologies in Metro 2033.

Idea is simple - render reflection into gbuffer with non-reflected attributes, and light both scene and reflected scene in the next step. There are some subtleties, but in general it's easy to implement. Also there was some troubles with non-lighted objects, like sky and glass there, but it can be solved by preservation of depth buffer during rendering scene into gbuffers.

&nbsp;
