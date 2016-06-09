---
layout: tool
title: Bone Chain Renamer
lang: fr
ref: bonechainrenamer
permalink: /tools/BoneChainRenamer-fr/
cat: rigging
stable_version: N/A
stable_status: Pas encore publié
dev_version: 0.0.1
dev_status: En développement
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
Si vous ne savez pas installer un Addon, suivez la [procédure suivante]({{site.base_url}}/AddonInstallation-fr/).  

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
  * Les chaines sont numérotées dans l'ordre alphabétique de leur os racine respectif. Vous pouvez au préalable les renommer  *a, b, c, ...* si vous voulez choisir l'ordre des chaines.  
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
