---
layout: post
title: Cinematic effects
date: 2013-12-02 05:13
author: admin
comments: true
categories: [game, iron cube, engine]
youtubeId: Wg4ERZKFAF8
---
I am reading books and articles about mobile/indie game marketing, and it's quite interesting. One of the most important things for game marketing is a good trailer, so I decided to add movie recording/playback to Iron Cube and Glow engine.

The task looked complicated but actually has simple solution - to record a game you just need to save all incoming data from a server to a client. Later, in the editor, you can just load this file and emulate network communication from the server to restore the original game. It automatically becomes compressed, because I'm using a snapshot-based system for networking in Glow engine and only changed data is sent between the server and client. For example the movie below is less than 1 MB.

And this allows many interesting options - for example you can reduce the speed of playback to have Matrix-like slow motion!


{% include youtubePlayer.html id=page.youtubeId %}

There is no interpolation between frames, so it may look slightly laggy.
