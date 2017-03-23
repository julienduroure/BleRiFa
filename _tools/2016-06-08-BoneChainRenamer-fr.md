---
layout: tool
title: Bone Chain Renamer
lang: fr
ref: bonechainrenamer
permalink: /fr/tools/BoneChainRenamer/
redirect_from:
  - /tools/BoneChainRenamer-fr/
cat: rigging
sort_nb: 6
stable_version: N/A
stable_status: Pas encore publié
dev_version: 0.0.1
dev_status: En développement / Beta privée à la demande
description: Renommez facilement vos chaines d'os
img: BoneChainRenamer.png
getit_url:
  - label: item 1
    url: http://google.com/1
  - label: item 2
    url: http://google.com/2
display_url: false
---

# Pour démarrer
Si vous ne savez pas installer un Addon, suivez la [procédure suivante][1].  

# Aperçu

{% include html5video.html id="BoneChainRenamer.ogv" %}

# Comment ça marche

* Il faut tout d'abord renommer l'os racine de votre première chaine : par exemple *finger.R*  
*BoneChainRenamer va reconnaitre automatiquement si ce nom comporte un suffixe gauche/droite '.R'.*  
<br/>
* Sélectionnez tous les os root de vos chaines, en sélectionnant en dernier l'os renommé à l'étape 1.  
<br/>
* Lancez BoneChainRenamer. Les chaines sont maintenant renommé avec les règls suivantes :  
<br/>
  * La 1ère chaine est maintenant *finger_0.R* (et les autres os de la chaine *finger_0.R.001*, etc...)  
<br/>
  * Les autres chaines sont *finger_1.R* (et *finger_1.R.001*, etc...), *finger_2.R* (et *finger_2.R.001*, etc...)  
<br/>
  * Des options sont disponibles dans les préférences de l'Addon (voir plus bas)  
<br/>
* Les chaines sont renommées suivant un tri basé sur l'os racine de la chaine. Dans les propriétés de l'opérateur, on peut choisir le type de tri que l'on veut appliquer :    
  * Alphabetic: _basé sur le nom des os_
  * X location: _basé sur la position X des os (espace d'évaluation 'World') : par ordre croissant_
  * Y location: _basé sur la position Y des os (espace d'évaluation 'World') : par ordre croissant_
  * Z location: _basé sur la position Z des os (espace d'évaluation 'World') : par ordre croissant_
  * X location reversed: _basé sur la position X des os (espace d'évaluation 'World') : par ordre décroissant_
  * Y location reversed: _basé sur la position Y des os (espace d'évaluation 'World') : par ordre décroissant_
  * Z location reversed: _basé sur la position Z des os (espace d'évaluation 'World') : par ordre décroissant_
  * Distance: _basé sur la distance entre les os et l'os actif : par distance croissante_
  * Distance reversed: _basé sur la distance entre les os et l'os actif : par distance décroissante_

For distances (_Distance_ and _Distance reversed), distance is based on "center" of bones (median point between head and tail), in order to be able to rename in such cases :  
![][2]
<br/>
  * Pour chaque chaine, le renommage s'arrête lorsqu'un os a plusieurs enfants.  
<br/>
![Stop when forks]({{site.base_url}}/assets/img/BoneChainRenamer/stop_when_forks.png)
<br/>

# Préférences

![Preferences]({{site.base_url}}/assets/img/BoneChainRenamer/preferences.png)

* *Séparator* : *Underscore* par défaut. La chaine de caractère utilisée pour séparer le nom de la chaine et son numéro  
<br/>
* *Count* : Comment les chaines sont numérotées/identifiées. Numérique par défaut : *finger_0.R, finger_1.R, finger_2.R*, etc...  
Cela peut être changé en alphanumérique : *finger_a.R, finger_b.R, finger_c.R*, etc...  
<br/>
![With letters]({{site.base_url}}/assets/img/BoneChainRenamer/with_letters.png)
<br/>
* *No count when single chain rename*: Si un seul os est sélectionné, il est possible de le renommer *finger.R* au lieu de *finger_0.R*  
<br/>
* *Stop chain when bone is not connected* : Il est possible de choisir si le renommage s'arrête si un os est parenté mais non connecté à son parent, ou bien si la chaine continue jusqu'à ce qu'un os n'est pas d'enfant.


[1]: {{site.base_url}}/fr/AddonInstallation/
[2]: {{site.base_url}}/assets/img/BoneChainRenamer/by_distance.png
