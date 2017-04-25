---
layout: post
title: TBB adopted
date: 2011-02-02 08:22
author: admin
comments: true
categories: [engine]
---
Embedding of Intel Threading Building Blocks is finished, really good library  with many abilities.  <br />  Development of a concurrent scene graph  is started, scene graph (sectors - portals) was made templated, to hold different types of objects and it supports now read-only access from several threads (or tasks). Also several modules of engine have copy of the scene graph  - renderer holds scene graph with visible objects, physics - with physical to optimize simulation.
