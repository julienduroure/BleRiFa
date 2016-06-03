---
layout: tool
title: AutoRefSpace
lang: en
ref: autorefspace
permalink: /tools/AutoRefSpace/
cat: rigging
stable_version: N/A
stable_status: Not yet released
dev_version: 0.0.1
dev_status: In development
description: Auto choose your bone reference spaces
img: autorefspace.png
getit_url:
  - label: item 1
    url: http://google.com/1
  - label: item 2
    url: http://google.com/2
display_url: false
---

## Getting Started
If you don't know how to install Addon, read [following documentation]({{site.base_url}}/AddonInstallation/).  

## Overview
{% include html5video.html id="AutoRefSpace_1.ogv" %}

## Reference System

### Adding Reference System

There are multiple way to create a new system:  

* If no bones are selected, this will create an empty system  
![System]({{site.base_url}}/assets/img/AutoRefSpace/reference_system.png)  
<br/>
* If bone(s) are selected, this will create a new system and fill data:  
![System Detail]({{site.base_url}}/assets/img/AutoRefSpace/system_detail.png)  
<br/>
  * Active bone (last selected) will be set as Bone that will have RefSpace  
  * Selected bones (but not active) will be set as Reference bones  
<br/>
* You can copy an existing Reference System  
* You can mirror copy an existing Reference System  
![Copy]({{site.base_url}}/assets/img/AutoRefSpace/system_copy.png)  

### Data in Reference System

* Label: Label of dropdown list that will be created
* Bone: Bone that will have a dynamic Reference space
* Reference Bones: List of Reference bones of bone 'Bone'. There is multiple way to fill them:  
  * Select all corresponding bones, and click on 'Fill from Selection'  
  * Click on '+' button, and fill name of bone at bottom of list, or click on bone icon when your bone is active.  
*  Reference Bone Labels: For each Reference Bone, you can choose a label that will be displayed in dropdown list. By default, labels are bone names.  
![System Detail]({{site.base_url}}/assets/img/AutoRefSpace/system_detail_2.png)  

### Activate Reference system

![Activate]({{site.base_url}}/assets/img/AutoRefSpace/active_autoref.png)  
<br/>
This will activate your corresponding Reference System. A dropdown list is now displayed (with labels filled).  
<br/>
![Choose]({{site.base_url}}/assets/img/AutoRefSpace/choose_ref.png)  
<br/>
You can now change Reference Space for your bone.  
Click on 'activate' again to disable dynamic references, and be able to perform modification on this system.  
**Note that is mode is only used for tests. Do not try to insert keyframes on this dropdown list.**  
Use 'Generation' to continue process, and be able to insert keyframes on Reference Space.

### Generation

![Generate]({{site.base_url}}/assets/img/AutoRefSpace/generate.png)  
<br/>
Clicking on 'Generate' will create a new panel with dropdown list for all your Reference System (not only active one, as it can be with 'activate').  
Corresponding dropdown lists are displayed only when bone(s) is/are selected.  
<br/>
![choose_]({{site.base_url}}/assets/img/AutoRefSpace/generated_ref_choose.png)  
<br/>
![chooses_]({{site.base_url}}/assets/img/AutoRefSpace/generated_ref_chooses.png)  
<br/>
You can choose where this panel will be displayed (tool or property sidebar of 3D View).  
![view_location]({{site.base_url}}/assets/img/AutoRefSpace/view_location.png)  
<br/>
*If data are empty, data from Addon Preferences will be used*  
<br/>
Once Generated, Reference systems can't be edited anymore. You have to click on 'update' if you want to update your data, and click on 'Generate' again.  
<br/>
![update]({{site.base_url}}/assets/img/AutoRefSpace/update.png)  
<br/>
**Once generated, this Addon is no more used, and you can now use Reference Space changes on all Blender installation, without need of install/share the addon with .blend file.**

### Addon Preferences

On left side, you can choose :
![pref_1]({{site.base_url}}/assets/img/AutoRefSpace/preferences_1.png)  

* Which tab of tool sidebar will display this Addon (before generating).  
* Default data used for generation if you leave them empty.  

On right side, data used for mirror copy:  
![pref_2]({{site.base_url}}/assets/img/AutoRefSpace/preferences_2.png)  
Default data are filled when you first create a Reference System, or by clicking on button 'Init Sides'.  
On created table, you can manage side suffix used on your rig.  
By default, common suffixes used are already filled.  
