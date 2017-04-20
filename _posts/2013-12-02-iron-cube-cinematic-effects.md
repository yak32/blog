---
layout: post
title: Iron Cube, cinematic effects
date: 2013-12-02 05:13
author: admin
comments: true
categories: [Uncategorized]
---
<p style="text-align: justify;">I am reading books and articles about mobile/indie game marketing, it's quite interesting. One of most important things for game marketing is good trailer, so I decided to add movie recording/playback to Iron Cube and Glow engine.</p>
<p style="text-align: justify;">The task looked complicated but actually has simple solution - to record game you need just save all incoming data from server on a client. Later, in the editor, you can just load this file and emulate network communication from the server to restore original game. And it's automatically became compressed, because I am using snapshot-based system for networking in Glow engine and only changed data is sent between server and client. For example movie below is less than 1 MB.</p>
<p style="text-align: justify;">And this way allows many interesting options - for example you can reduce speed of playback to have "Matrix"-like slow motion!</p>
<iframe src="//www.youtube.com/embed/Wg4ERZKFAF8?rel=0" height="360" width="640" allowfullscreen="" frameborder="0"></iframe>
There is no interpolation between frames, so it may look slightly laggy.
