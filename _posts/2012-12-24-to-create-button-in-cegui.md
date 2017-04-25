---
layout: post
title: CEGUI vs IMGUI
subtitle: Bloated UI
date: 2012-12-24 10:58
author: admin
comments: true
categories: [engine]
---
Code of button creation in CEGUI:

```C++

  // Create Window
wnd = CEGUI::WindowManager::getSingleton().createWindow(TaharezLook/Button,JumpPushButton);
wnd->setPosition(CEGUI::UVector2(CEGUI::UDim(0.75,0),CEGUI::UDim(0.50,0)));
wnd->setSize(CEGUI::UVector2(CEGUI::UDim(0,50),CEGUI::UDim(0,50)));
wnd->setText(Jump!);
CEGUI::System::getSingleton().getGUISheet()->addChildWindow(gJumpBtnWindow);
```

It's really ugly. Reminds me joke by Charlie Bloom.
<a href="http://cbloomrants.blogspot.kr/2012/12/12-15-12-how-to-lose-game-developer-love.html">http://cbloomrants.blogspot.kr/2012/12/12-15-12-how-to-lose-game-developer-love.html</a>

How creation and button usage should look like:

```C++
if ( gui.button(Cancel)  )
   cancel_job();
```
