---
layout: post
title: moving to Intel Threading Blocks
date: 2011-01-31 05:22
author: admin
comments: true
categories: [engine]
---
deeper and deeper into concurrency and multi threading... <br />  I have decision to use <a href="http://www.threadingbuildingblocks.org/">Intel Threading Building Blocks</a> instead of   experimental  <a href="http://threadpool.sourceforge.net/">boost::thread_pool</a>.  All computations in the Glow engine are organized into tasks and theoretically would scale well when number of hardware threads (CPU cores) will be increased.   <br />  Previously, I used boost::thread_pool for task execution. Now, when I returned to concurrency, I realized that usage of boost::thread_pool is not scalable, because it heavily uses mutexes (spin-based). Later I will launch tests to measure scalability of both methods and post results here.
