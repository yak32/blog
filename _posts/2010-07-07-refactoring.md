---
layout: post
title: Refactoring
date: 2010-07-07 06:26
author: admin
comments: true
categories: [Uncategorized]
---
I spent a month on refactoring of engine. It's became so big, I can not serve it in my little brain.  <br />  So I detached it into small pieces, like physics, sound,   networking, core, ai, ui, archive, prepared solid interface to  access features of engine (which will be visible for users of  engine). Also put all pieces into dll, and prepare abstract   interface for every module to clearly isolate it.   <br />  Also the thread pool (boost::threadpool) is added to execute jobs from modules.  So now engine will scale performance easily with more CPU cores.<span class="Apple-tab-span" style="white-space:pre"> </span>
