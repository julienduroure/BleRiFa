---
layout: tool
title: FrameShift
lang: en
ref: FrameShift
permalink: /tools/FrameShift/
cat: animation
stable_version: N/A
stable_status: Not yet released
dev_version: 0.0.1
dev_status: In development
description: Shifting frames for timing process
img: FrameShift.png
getit_url:
  - label: item 1
    url: http://google.com/1
  - label: item 2
    url: http://google.com/2
display_url: false
---

# Getting Started
If you don't know how to install Addon, read [following documentation][1].  

# Overview

FramShift is used to shift easily frames (forward or backward).    

{% include html5video.html id="FrameShift_1.ogv" %}

# How it works

Currently, this addon works only on pose mode (so only for rigs).  

## Where ?

It can be used:  

* On DopeSheet
* On GraphEditor
* On TimeLine
*	On 3D View

## How ?
When pressing Shift+Q, it will shift foreward all keyframes that are next to current frame.
Pressing Alt+Shift+Q will shift backward all keyframes next to current one. If you try to go backward to much, addon will not let you delete keyframes or overlap between them.

## How many ?
Number of frame to shift is defined in operator parameters. By defaut, is set to 1.  
When you changed it (after using Shilf+Q or Alt+Shift+Q), frame number is saved, and this new value will be used for next call of operator. You can also change backward/foreward.  

![OpsParameter]({{site.base_url}}/assets/img/FrameShift/OpsParameters.png)

# Addon Preferences
![AddonPref]({{site.base_url}}/assets/img/FrameShift/AddonPref.png)
* You can change key shortcut  
* You can choose if shifting is applied only on selected bones, or on entire rig.  

# How to report bugs or request new features ?
You can report bugs on [Issue Tracker][2]

[1]: {{site.base_url}}/AddonInstallation/
[2]: https://github.com/julienduroure/BleRiFa/issues/
