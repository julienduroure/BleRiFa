---
layout: post
title: Summer Dev Update
lang: en
ref: dev_update
img: 20161214_dev_update.png
permalink: /en/:year/:month/summer-dev-update/
redirect_from:
  - /2016/09/14/summer-dev-update/
version: 3
---

Hi all,
Here is some quick news of state of development. I didn't post news recently, but development is in progress :)

# [ExtraGroups][1]

##  Access bone properties
A new operator is coming: you are now be able to access directly to all bone properties of all bones of your group.

{% include html5video.html id="bone_properties.ogv" %}
<br/>
<br/>  

##  Using KeyingSets
You can now link your groups to KeyingSets. When you select your group, corresponding KeyingSet is automatically selected.  
If you add a group to selection, a new composite KeyingSet is automatically created, with channels from old and new groups added.  
What should happened when you remove from selection is not developed yet, and this feature should be discussed :)

{% include html5video.html id="group_keyingset.ogv" %}
<br/>
<br/>  

# [AutoSnap][2]
FK/IK switch can now be driven by a bone transformation, instead of bone property.

{% include html5video.html id="switch_bone_transformation.ogv" %}

[1]: {{site.base_url}}/en/tools/ExtraGroups/
[2]: {{site.base_url}}/en/tools/AutoSnap/
