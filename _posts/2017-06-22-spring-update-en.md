---
layout: post
title: "Spring 2017: updates"
lang: en
ref: 2017-spring-update
img: 20161214_dev_update.png
permalink: /en/:year/:month/2017-spring-update/
version: 1
---

What's new on BleriFa ?

# [ExtraGroups][1]

![][15]

ExtraGroups v1.0 is now released!  
The [documentation][1] is now completed, and the addon is available on [BlenderMarket][2] and [Gumroad][3]

*  Now possible to display as popup
*  Copy group / Copy mirror group
*  New operator: Motion Path
*  Select & Visibility are now displayed by default at initialisation
*  Ops are now displayed always at same order at initialisation
*  Name clickable option
*  Event system:  
	*	New mode for selection: Select and hide others
	*  New mode for selection: Select opposite
	*  Display label instead of mode directly
	*  Possibility to active/deactivate events for each operator
	*  Solo mode for Lock ops
	*  Mirror events for all ops
*  Manipulator management for selection (gizmo / axes)
*  Store/restore/change active bone of each group
*  Import / Export:
	*  color / gizmo / axes / active bone
	*  import/export what ops are displayed
	*  import/export order of ops
* color management directly in UI / only editable on edit mode
* Better UI for all addon preferences / options, ...
* Non blocking solo mode
* Some bug fixing here and there


# [AutoRefSpace][4]
*  Completly new system to avoid some matrix issue (when using _Selection to cursor_). No user interface difference, but core stuff is completly new. Still need some work before a first private beta release.  
{% include html5video.html id="AutoRefSpace_1.ogv" %}

# [PanelMaker][5]
*  It's now possible to create interface for any properties of any objects of your scene.

{% include html5video.html id="PanelMaker_2.ogv" %}

# [FrameShift][10]
*  I added a new tool used to [shift frames][10]  

{% include html5video.html id="FrameShift_1.ogv" %}

# [FootRollBreak][6]
*  FootRollBreak is now available on [Gumroad][11] too
*  Updating [documentation][6] to explain how to use FootRollBreak on linked rigs.

# [Mass KeyingSet][7]
*  This addon is now available on [BlenderMarket][8] and [Gumroad][9]

# On BleRiFa website
*  Some layout updates here and there
*  Tools are now displayed on homepage with tiles layout
*  Massive refactoring of permalinks
*  And a new blog post about [ExtraGroups v1.0 release][12]

# On Julien Duroure website
*  [10 checks to perform on Rigs][13]
*  [Weather animation tutorial][14]

[1]: {{site.base_url}}/en/tools/ExtraGroups/
[2]: https://blendermarket.com/products/extragroups
[3]: https://gumroad.com/l/ExtraGroups
[4]: {{site.base_url}}/en/tools/AutoRefSpace/
[5]: {{site.base_url}}/en/tools/PanelMaker/
[6]: {{site.base_url}}/en/tools/FootRollBreak/
[7]: {{site.base_url}}/en/tools/MassKeyingSets/
[8]: https://blendermarket.com/products/mass-keyingsets
[9]: https://gumroad.com/l/SRqtl
[10]: {{site.base_url}}/en/tools/FrameShift/
[11]: https://gumroad.com/l/FootRollBreak
[12]: {{site.base_url}}/en/2017/05/ExtraGroups-V1-release/
[13]: http://julienduroure.com/en/2017/05/10-checks-on-rigs/
[14]: http://julienduroure.com/en/2017/06/weather-anim-tuto/
[15]: {{site.base_url}}/assets/img/ExtraGroups/popup.png
