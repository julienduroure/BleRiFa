---
layout: tool
title: "Bone Picker"
lang: en
ref: BonePicker
permalink: /en/tools/BonePicker/
cat: rigging
sort_nb: 4
stable_version: 0.0.1 (alpha version)
stable_status: Public alpha version
dev_version: 0.0.2
dev_status: In development
description: Select your superimposed bones
img: BonePicker.png
getit_url:
  - label: Gumroad
    url: https://gumroad.com/l/BonePicker
display_url: true
---

# Getting Started
If you don't know how to install Addon, read [following documentation][1].  

# Overview

This addon is used to easily select your superimposed bones.  
You can also know your superimposed bones, but not selectables (because of layer or hidden stuff).

![]({{site.base_url}}/assets/img/BonePicker/popup.png)

{% include html5video.html id="BonePicker.ogv" %}

# How it works

When you display the popup (activated with keyboard shortcut, defined in addon preferences), you can:  


*  Select a bone with Left Mouse Button
*  Add bone to select with Shift
*  UnSelect with clicking again on bone.


You can see:  

*  Bones that are currently selected
*  Active bone  

You can also see (about non selectable bones):  

*  Hidden Superimposed bones
*  Superimposed bones that are on another layer


# Options

Keyboard shortcut can be modified in addon preferences.  
You can also modify threshold for superimposed detection.

![]({{site.base_url}}/assets/img/BonePicker/UserPref.png)

# How to report bugs or request new features ?
You can report bugs on [Issue Tracker][2]

[1]: {{site.base_url}}/fr/AddonInstallation/
[2]: https://github.com/julienduroure/BleRiFa/issues/
