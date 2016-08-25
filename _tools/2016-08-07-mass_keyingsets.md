---
layout: tool
title: Mass KeyingSets
lang: en
ref: masskeyingsets
permalink: /tools/MassKeyingSets/
cat: animation
stable_version: 0.1.0 (beta version)
stable_status: Beta version 0.1.0 is public available
dev_version: 0.1.0
dev_status: In development / stabilisation
description: Mass creation of KeyingSets
img: MassKeyingSets.png
getit_url:
- label: Google Drive
  url: https://drive.google.com/open?id=0B-mpivl1jPpuNUJGYmVVeGVDSDQ
display_url: true
---

## Getting Started

If you don't know how to install Addon, read [following documentation][1].  

## Overview

![Panel]({{site.base_url}}/assets/img/MassKeyingSets/panel.png)  
<br/>
A new panel is added on Scene properties (with other KeyingSets stuff), only when:  
* You are in pose mode on armature, with at least one bone selected  
* You are in object mode, with at least one object selected  

When you click on button, a popup lets you choose what you want to put into keyingset.  
There is two different popup, depending on mode you are (pose mode or object mode)  

![Bones]({{site.base_url}}/assets/img/MassKeyingSets/popup_bones.png)  
<br/>
![Objects]({{site.base_url}}/assets/img/MassKeyingSets/popup_objects.png)  

## Options

# Name  

Name of KeyingSet you are going to create.

# Location, Rotation, Scale

Channel(s) you want to include into keyingset.

# Bone Custom Properties

Add all custom properties defined at bone level (of selected bones) into keyingset

# Object Custom Properties

Add all custom properties defined at object level (of selected objects) into keyingset

# Object Data Custom Properties

Add all custom properties defined at object data level (of selected objects) into keyingset :  
At mesh level for mesh objects, curve data for bezier curves, etc...

## How to report bugs or request new features ?
You can report bugs on [Issue Tracker][2]

[1]: {{site.base_url}}/AddonInstallation/
[2]: https://github.com/julienduroure/MassKeyingSets/issues/
