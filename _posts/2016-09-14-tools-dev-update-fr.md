---
layout: post
title: Développement de l'été
lang: fr
ref: dev_update
img: 20161214_dev_update.png
permalink: /fr/:year/:month/developpement-ete/
redirect_from:
  - /2016/09/14/developpement-ete/
version: 3
---

Bonjour à tous,
Même si je n'ai pas été très bavard cet été, le développement continue :) Voici quelques améliorations :

# [ExtraGroups][1]

##  Access bone properties
Un nouvel opérateur est disponible : il permet d'accéder directement aux propriétés des os du groupe.

{% include html5video.html id="bone_properties.ogv" %}
<br/>
<br/>  

##  _KeyingSets_
On peut maintenant lier un groupe à un _KeyingSet_. Quand on sélectionne le groupe, le _KeyingSet_ correspondant est automatiquement sélectionné.  
Si on ajoute un groupe à la sélection, un _KeyingSet_ particulier est automatiquement créé, il contient l'ensemble des canaux de la nouvelle sélection.  
Ce qui doit se passer quand on soustrait de la sélection reste à coder (et à définir surtout).  

{% include html5video.html id="group_keyingset.ogv" %}
<br/>
<br/>  

# [AutoSnap][2]
On peut maintenant utiliser la position/rotation/mise à l'échelle pour définir un switch, si vous préférer cette solution à l'utilisation d'une propriété.

{% include html5video.html id="switch_bone_transformation.ogv" %}

[1]: {{site.base_url}}/fr/tools/ExtraGroups/
[2]: {{site.base_url}}/fr/tools/AutoSnap/
