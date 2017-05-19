---
layout: tool
title: ExtraGroups
lang: en
ref: ExtraGroups
permalink: /en/tools/ExtraGroups/
redirect_from:
  - /tools/ExtraGroups/
cat: animation
sort_nb: 1
stable_version: 1.0.0
stable_status: Published on 2017 May, 20th
dev_version: 1.0.1 (bug fixing release) / 1.1 (feature release)
dev_status: In active development
description: Enhance your animation workflow!
img: ExtraGroups.png
getit_url:
  - label: Gumroad
    url: https://gumroad.com/l/ExtraGroups
  - label: BlenderMarket (when validated...)
    url: https://blendermarket.com/products/extragroups
display_url: true
---

## Getting Started
If you don't know how to install Addon, read [following documentation][1].  

## Presentation  

This Addon is used to manage set of bones, during animation (pose mode).  
You can manage your bone groups (create / delete / sort groups, and adding / removing bone(s) from groups).  
For each group, you can use some operators (you can customize which one are displayed, and in which order).    

![][22]

{% include youtube.html id='Ljteyl8XUFM' %}

## Starting with ExtraGroups

![][4]

If your are new using this addon, click on "Create from scratch" to setup default data.  
If you know what you are doing, see _Import / Export_ manual.  

## Manage your groups

![][3]

Note that you can manage your groups only on edit mode:  

![][5]

# Create groups

When you create a group, all selected bones are automatically added to this newly created group. Note that a bone can belong to more than a group.  
For each group, you can defined what is your main bone of the group. When you are creating a group, the main bone is the active bone of your selection.  

# Delete groups

The group is deleted. Bone properties that can have been changed by operator are not restored.  

# Update groups

*  Adding bones to current group: All selected bones are added to the current group.  
*  Deleting bones from current group: All selected bones are removed from the current group.  

# Copy groups & Mirror copy groups

![][6]

*  Copy group
The group is copied: bone list, and corresponding properties
*  Mirror copy group
The group is copied. All sided bones (for example with _.L_ suffix) are mirrored, other ones are kept same. If suffix of the group name is also sided, your newly created group will be mirrored too.  

# Current selection group

Available by default, the "current selection" group is a special group, that always contains your current bone selection. So you can't add or remove bones from this group.  
Note that some operators are not available for this special group.  

If you delete this group, a new button is available to be able to add it again.  

![][7]
<br/>
<br/>
## Manage your operators

![][8]

Operators are action that you will be able to perform on your groups (even if bones from this group are not selected in 3D view).  
Note that you can manage your operators only on edit mode.  

# Displayed or not displayed ?

You can decide which operators are displayed or not. Don't display tools you will not use!  
By default, _selection_ and _visibility_ operators are displayed.

# Sort your operators

You can sort your operator in this list. Corresponding order will be used on panel and popup :)

# Adding / removing operators

Adding operators is only available on _developper mode_ (see addon preferences).  
Only operators that are created by user (so in _developper mode_) can be removed.

# Change icons

You can change icons of each operator.  
For _action_ operator, you will have 1 icon. For _toggle_ operator, you will have 2 icons (one for _on_, one for _off_).  

You can change icon direcly by typing the name (if you know it), or by picking icon in list (available by clicking on small triangle).  

![][9]

# operator details

Some operator detail can be displayed:
*  Event / mode management (see below).
*  If operator is available for _current selection_ group.
*  Some technical stuff only displayed on _developper mode_.

## Manage your mode / events

![][10]

For each operator, you may want difference behavior. For example, for _selection_ operator, you may want to select only your group, to add your group to selection, or to select only your group, and hide all other bones. All these _modes_ can be used using only one operator, with modifier keys (Ctrl, Shift, Alt, ...).   

# activate your events

For each operator, you can decide which mode/event are enabled, which are not.

# manage your shortcuts

For each mode, you can decide what are the corresponding modifier keys.  
If you have more than one mode linked to only one event, a warning is displayed.

![][11]

## Available operators

Here is list of all available operators, and corresponding modes:  
Note that most of modes are also available in _mirror mode_ version (that means that operator will apply in mirror bones of the group)

#  Selection
* Select only
Will select your group only (other bones are de-selected).  
* Add to selection
Will add your group to your current selection.  
* Remove from selection
Will remove your group from your current selection.  
* Select only and hide others
Will select your group only (other bones are de-selected and hidden).  
* Select opposite
Will deselect your group, and select all other ones.  

# Mute
* Mute
Will mute animation of each bones of the group
* Solo mode
Will mute animation of each bone that is not from your group.

# Visibility
* Toggle visiblity
Will hide bones of your group if they are visible, will unhide if bones are hidden.
* Solo mode
Will hide all bones that are not from your group.

# Restrict Selection
* Toogle
Will toggle selection property of bones of your group.
* Solo mode
Will make unselectable bones that are not from your group.

# Proporties
Will display a popup where bone properties can be changed

# Lock
Will lock channels of bones from your group (no more possible to add keyframes)

# Keyframing
* Default
Will add keyframes on bones of your group, using KeyingSet set for your group (see option). If no keyingset is filled on your group option, menu will be displayed to choose your keyframe channels.
* Forced menu
Will add keyframes on bones of your group, displaying the keyframe menu, even if you set a keyingset on your group (see options)
* Keying Only
Will add keyframes on bones of your group, using KeyingSet set for your group (see option). If no keyingset is filled on your group option, no keyframes are added.

# Motion Path
* Add/Remove motion path
Will toogle motion path for bones of your group.
* update motion path
Will update motion path for bone of your group.

## Options

![][12]

# KeyingSet Management

![][13]

You can choose an existing KeyingSet linked to a group. If KeyingSet management is on, and a keyingset is filled:
*  Using _selection_ operator, this will change automatically your active keyingset
*  Using _Keyframing_ operator, this will use the keyingset to insert keyframes (except if you use _Forced Menu_ mode).

# Transformation Gizmo Management
![][14]

You can choose transformation gizmo and axis that will be automatically set when using _Selection_ operator.

# Color Label
![][15]

You can decide to use color label to save time (no need to read group name ;-)  
Color can be changed only in edit mode.  

# Multitype
![][16] ![][17]  
You can decide to split your groups into several "grouptype". For each type of "group of group" (each group type), you can have different opeator list and order.  

For popup, by default the grouptype list is not displayed, but available via the corresponding button.  
![][18] ![][19]

# Clickable name

When you activate this feature, the name of the group (in the list) is clickable. You can decide what operator will be used. Two solutions about the mode:  
*  You can decide what mode will be used when you click (and no modifier keys are enabled)  
  ![][20]
*  You can choose to use same events than legacy operator (the one available on icon)  
  ![][21]

## Import / Export

Import / Export is available when the corresponding checkbox is filled.  
![][23]

# Export to File
You can export your data to a text file. Most of addon data are exported:
*  Bone groups, and corresponding bones that belong to groups
*  Operators (sorting and which ones are displayed)
*  Most of options (color, gizmo, keyingset, clickable name data)

# Import from Bone Groups
If you defined some Bone Groups (Blender feature), you can create automatically bone groups (in ExtraGroups) from them.

# Import from Selection Sets
If you defined some Selection Sets (from Blender addon _Selection Sets_), you can create automatically bone groups (in ExtraGroups) from them.

# Import from KeyingSets
If some KeyingSets are defined on your rig, you can create automatically bone groups from bones involded in keyingsets.

# Import from File
You can import data from file, that you generated using _Export to File_. (Please use same version of addon for better results).

## Using this addon with linked rigs
You can use ExtraGroups addon with linked rigs. Let's say that you have a _Rig_ file, where your rig is, and an _animation file_, where your rig is linked, and where you are doing the animation. You have to do in 2 steps:
*  Create your ExtraGroups data on your rig file (groups, operators, events)
*  On you animation file, when you activate ExtraGroups addon on a linked (and proxyfied) armature, you will see that ExtraGroups are automatically imported into your animation file.
*  If you want to change some data (operator displayed, add a new group, change bones in group, etc...), you can do in directly into your animation file, if you need it only on this animation file.
*  If the rig is used in multiple animation file, you need to perform changes into rig file. In your animation file, on _edit mode_, you will find a new panel with a button to import ExtraGroups data from rig file to animation file.  
  ![][24]

## Developper mode

Developper mode, available in Addon User Preferences, is used to create your own operator. Not sure this feature is quite stable. So I am not going to document it, let's say that it will not invite you to use it ;-)

## Addon Preferences

![][25]

# Display
You can choose to active (or not) the popup. And you can choose your hotkey for it.  
You can also choose the tab where addon is displayed.

# Developper mode
If you really really really want to use it, please contact me, I will explain you.

# Danger zone
If something got wrong, you can delete all data of ExtraGroups from your current file.

## Updating this addon

There is no auto-update on this addon (for now). So you can update by:  
*  de-activate the addon
* remove it
* install new version
* activate the new version

For some updates, some internal data storage update are needed. That means that these updates must be done before you can use the new version. Don't worry, it won't be hard.

# For local rigs
No link system! Easy case :)  
Instead of your usual addon panels, you will find a button, asking you to update data. Click, and that's it :)

![][26]

# For linked rigs
You will have to update your rig file first. Then, you can update your animation file.

![][27]

So, steps are:
*  Update addon
*  Close your animation file
*  Open your rig file
*  Update addon data by clicking on button asking you to update
*  Save your rig file, and close it
*  Open again your animation file
*  This time, you can reload data from library
*  Save your file!

## How to report bugs or request new features ?
You can report bugs on [Issue Tracker][2]

## Version history
*  __v1.0.0__, 2017 may, 20th: initial release


[1]: {{site.base_url}}/en/AddonInstallation/
[2]: https://github.com/julienduroure/BleRiFa/issues/
[3]: {{site.base_url}}/assets/img/ExtraGroups/manage_groups.png
[4]: {{site.base_url}}/assets/img/ExtraGroups/init.png
[5]: {{site.base_url}}/assets/img/ExtraGroups/edit_mode.png
[6]: {{site.base_url}}/assets/img/ExtraGroups/copy_groups.png
[7]: {{site.base_url}}/assets/img/ExtraGroups/current_selection.png
[8]: {{site.base_url}}/assets/img/ExtraGroups/manage_operator.png
[9]: {{site.base_url}}/assets/img/ExtraGroups/icon_picking.png
[10]: {{site.base_url}}/assets/img/ExtraGroups/manage_event.png
[11]: {{site.base_url}}/assets/img/ExtraGroups/event_warning.png
[12]: {{site.base_url}}/assets/img/ExtraGroups/options.png
[13]: {{site.base_url}}/assets/img/ExtraGroups/keyingset.png
[14]: {{site.base_url}}/assets/img/ExtraGroups/gizmo.png
[15]: {{site.base_url}}/assets/img/ExtraGroups/colorlabel.png
[16]: {{site.base_url}}/assets/img/ExtraGroups/grouptype_legs.png
[17]: {{site.base_url}}/assets/img/ExtraGroups/grouptype_arms.png
[18]: {{site.base_url}}/assets/img/ExtraGroups/grouptype_popup_1.png
[19]: {{site.base_url}}/assets/img/ExtraGroups/grouptype_popup_2.png
[20]: {{site.base_url}}/assets/img/ExtraGroups/name_clickable_1.png
[21]: {{site.base_url}}/assets/img/ExtraGroups/name_clickable_2.png
[22]: {{site.base_url}}/assets/img/ExtraGroups/popup.png
[23]: {{site.base_url}}/assets/img/ExtraGroups/import_export.png
[24]: {{site.base_url}}/assets/img/ExtraGroups/linked_reload.png
[25]: {{site.base_url}}/assets/img/ExtraGroups/addonpreferences.png
[26]: {{site.base_url}}/assets/img/ExtraGroups/update_addon.png
[27]: {{site.base_url}}/assets/img/ExtraGroups/reload_library_update.png
