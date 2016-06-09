---
layout: tool
title: Bone Chain Renamer
lang: en
ref: bonechainrenamer
permalink: /tools/BoneChainRenamer/
cat: rigging
stable_version: N/A
stable_status: Not yet released
dev_version: 0.0.1
dev_status: In development
description: Rename easily your bone chains
img: BoneChainRenamer.png
getit_url:
  - label: item 1
    url: http://google.com/1
  - label: item 2
    url: http://google.com/2
display_url: false
---

# Getting Started
If you don't know how to install Addon, read [following documentation]({{site.base_url}}/AddonInstallation/).  

# Overview

{% include html5video.html id="BoneChainRenamer.ogv" %}

# How it works

* You need first to rename 1 bone to fit your requirements: You can choose for example *finger.R*  
*BoneChainRenamer will automatically find if there is a side suffix on your bone name (".R").*  
<br/>
* Select all your chain root bones, last selected must be your renamed root bone (at step 1).  
<br/>
* Launch BoneChainRenamer. Bone Chains are now renamed with following rules:  
<br/>
  * First chain is now finger_0.R (and other bones of this chain finger_0.R.001, etc...)  
<br/>
  * Other chains are named finger_1.R (and finger_1.R.001, etc...), finger_2.R (and finger_2.R.001, etc...)  
<br/>
  * See addon preferences for more information about separator, how to count chains, etc...  
<br/>
  * Chains are renamed based on alphabetic order of their root. You can optionally rename roots *a, b, c, ...* if you want to choose order of your chains  
<br/>
  * On a chain, renaming will stop when your chain forks  
<br/>
![Stop when forks]({{site.base_url}}/assets/img/BoneChainRenamer/stop_when_forks.png)
<br/>

# Addon Preferences

![Preferences]({{site.base_url}}/assets/img/BoneChainRenamer/preferences.png)

* Separator : *Underscore* by default. Character used to separate your chain name and chain counting  
<br/>
* Counting method : How to identify chains. Numeric by default : *finger_0.R, finger_1.R, finger_2.R*, etc...  
It can be changed to alphanumeric: *finger_a.R, finger_b.R, finger_c.R*, etc...  
<br/>
![With letters]({{site.base_url}}/assets/img/BoneChainRenamer/with_letters.png)  
<br/>
* No count when single chain rename: If you select only 1 root bone, you can choose if bones will be renamed *finger_0.R*, or only *finger.R*  
<br/>
* Stop chain when bone is not connected: You can choose if renaming stops when a bone is not connected to its parent, or if renaming continue until a bone has no child (connected or not)
