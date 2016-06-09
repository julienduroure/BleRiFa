---
layout: tool
title: FootRollBreak
lang: en
ref: footrollbreak
permalink: /tools/FootRollBreak/
cat: rigging
stable_version: 1.0.0
stable_status: Released on March 25th, 2016
dev_version: N/A
dev_status: No development in progress for now
description: Enhance your rigify rigs
img: FootRollBreak.png
getit_url:
  - label: Blender Market
    url: https://cgcookiemarkets.com/all-products/footrollbreak/
display_url: true
---

# Getting Started
If you don't know how to install Addon, read [following documentation]({{site.base_url}}/AddonInstallation/).  

# FootRollBreak
FootRollBreak is an addon that enhance Rigify rigs, adding FootRollBreak feature on existing rigify rigs.  
FootRollBreak let's your foot have a natural fold / unfold when you roll it.  

{% include html5video.html id='FootRollBreak.ogv' %}  

# Quick start

* Install FootRollBreak addon, and activate it.
* Select your rigify rig, and got to armature data properties. A new panel is there :)
* Patch your rig (works on both Human & Pitchipoy rigs)
* A new panel can be found on 3D View properties panels (N), near other rigify panels.
* That's it ! Enjoy :)
* FootRollBreak will remain enabled on your rig, even if you disable/remove the addon.

![angles]({{site.base_url}}/assets/img/FootRollBreak/angles.png)

# How to patch your rig ?

* Make sure that you select your rigify rig (not the metarig, the real rig, after rigify generation)
* On Armature Properties, find the new panel "Rigify FootRoll Break Patch"
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/addon_panel.png)  
<br/>
* Patch your rig by clicking on button "Patch FootRoll Break" (works on both Human & Pitchipoy rigs)
* Button is now replaced by a text "already patched!"
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/already_patched.png)  
<br/>
* Enter Edit Mode on armature, adjust new bone "toe-top" to define toe rotation pivot point. Back to pose mode.
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/toe-top.png)  
<br/>

# How to use your new FootRollBreak feature?

* FootRoll Break is Off by default. If you try to roll your foot, nothing happened.
* A new panel can be found on 3D View Properties  
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/ui_panel.png)  
<br/>
* Activate FootRollBreak (enable corresponding checkbox)  
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/footrollbreak_option.png)  
<br/>
* Try to roll your again :
  * At angle defined in parameter, your foot starts to take off, and your toes starts to unfold.
  * At "angle max", defined in parameter, your toes are totally unfolded.
  * In some uncommon cases, foot have some unnatural motion path. In that case, your case tweak "corrective angle" to have a better movement.  
<br/>
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/bad_motion.png)
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/correct_motion.png)

# Restrictions

Current version works only on biped rigify (default Rigify Rigs for example), but doesn't work with one-leg rigs, or more-than-2-legs rigs.

# How to report bugs ?
You can report bugs on [Issue Tracker](https://github.com/julienduroure/FootRollBreak/issues/)


# Version History
* v 1.0.0  
  * Date: 25 MARCH 2016
  * Change logs:
    * Initial release
