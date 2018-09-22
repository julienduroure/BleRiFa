---
layout: tool
title: Mass KeyingSets
lang: en
ref: masskeyingsets
permalink: /en/tools/MassKeyingSets/
redirect_from:
  - /tools/MassKeyingSets/
cat: animation
sort_nb: 2
stable_version: 0.2.0
stable_status: Version 0.1.0 is public available
dev_version: N/A
dev_status: N/A
description: Mass creation of KeyingSets
img: MassKeyingSets.png
getit_url:
- label: Blender Market
  url: https://blendermarket.com/products/mass-keyingsets
- label: Gumroad
  url: https://gumroad.com/l/SRqtl
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

When you click on the first button, a popup lets you choose what you want to put into keyingset.  
There is two different popup, depending on mode you are (pose mode or object mode)  

![Bones]({{site.base_url}}/assets/img/MassKeyingSets/popup_bones.png)  
<br/>
![Objects]({{site.base_url}}/assets/img/MassKeyingSets/popup_objects.png)  

When you click on second buttin, a KeyingSet is created, based on all properties already keyed (animated) in your scene.

## Options

# Update
If checked, the KeyingSet will be updated (instead of creation of a new keyingset)

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

## Version history
*  __v0.1.0__, 2016 august, 9th: initial release
*  __v0.2.0__, 2018 september, 22nd:  
    *  Bug fixing:
      *  Do not add keyingset for lock scale
    *  New features:
      *  A KeyingSet can now be updated
      *  Creation of KeyingSet from existing keyframed

[1]: {{site.base_url}}/en/AddonInstallation/
[2]: https://github.com/julienduroure/MassKeyingSets/issues/
