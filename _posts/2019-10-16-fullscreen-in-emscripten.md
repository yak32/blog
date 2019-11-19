---
layout: post
title: Running emscripten apps in fullscreen
subtitle:
date: 2019-10-16 12:13
author: admin
comments: true
categories: [ironcube, emscripten]
---

I spent an evening making my emscripten game demo working in full screen mode. So basically, Emscripen supports 2 modes - "proper" fullscreen, and soft fullscreen. First one is similiar to a fullscreen mode of a native app, but it seems not supported in all browsers. Soft fullscreen is just running the app fully resized in the browser window, and it's exactly what I needed.

![](/blog/images/uploads/2019/iron_cube_fullscreen.jpg){:class="img-responsive"}

It is 2 steps, assuming SDL2 usage for a platform layer:

1) switch to fullscreen after SDL window is created

```cpp
	if (fullscreen){
		EmscriptenFullscreenStrategy strategy;
		strategy.scaleMode = EMSCRIPTEN_FULLSCREEN_CANVAS_SCALE_STDDEF;
		strategy.filteringMode = EMSCRIPTEN_FULLSCREEN_FILTERING_DEFAULT;
		strategy.canvasResizedCallback = emscripten_window_resized_callback;
		strategy.canvasResizedCallbackUserData = this;   // pointer to user data
		emscripten_enter_soft_fullscreen("canvas", &strategy);
	}
```
"canvas" is the name of html element with game's main window (it's default in Emscripten shells)

2) create a callback to handle window resize event

```cpp
EM_BOOL emscripten_window_resized_callback(int eventType, const void *reserved, void *userData){
	METHOD();

	double width, height;
	emscripten_get_element_css_size("canvas", &width, &height);

	int w = (int)width, h = (int)height;

	// resize SDL window
	Platform* platform = (Platform*)userData;
	SDL_SetWindowSize((SDL_Window*)platform->get_wnd_handle(), w, h);

	// engine-specific code - internal render size should be updated here
	event_t e(ET_WINDOW_SIZE, w, h, timer::current_time());
	LOGI("Window resized to %dx%d", w, h);
	platform->on_window_size_changed(w, h);
	return true;
}
```
