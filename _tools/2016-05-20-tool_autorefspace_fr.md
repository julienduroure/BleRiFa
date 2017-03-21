---
layout: tool
title: AutoRefSpace
lang: fr
ref: autorefspace
permalink: /tools/AutoRefSpace-fr/
cat: rigging
sort_nb: 7
stable_version: N/A
stable_status: Pas encore publié
dev_version: 0.0.1
dev_status: En développement
description: Choisissez automatiquement l'espace de référence de vos os
img: autorefspace.png
getit_url:
  - label: item 1
    url: http://google.com/1
  - label: item 2
    url: http://google.com/2
display_url: false
---

## Pour démarrer
Si vous ne savez pas installer un Addon, suivez la [procédure suivante][1].  

## Vue d'ensemble
{% include html5video.html id="AutoRefSpace_1.ogv" %}

## Systèmes de Références

### Ajouter un nouveau système

Il y a plusieurs façons de créér un nouveau système :

* Si aucun os n'est sélectionné, cela va créer un système "vide", à compléter par la suite.
![System]({{site.base_url}}/assets/img/AutoRefSpace/reference_system.png)  
<br/>
* Si un ou plusieurs os sont sélectionnés, cela va créer un nouveau système, et remplir automatiquement les données :  
![System Detail]({{site.base_url}}/assets/img/AutoRefSpace/system_detail.png)  
<br/>
  * L'os actif (selectionné en dernier) sera défini comme l'os qui va pouvoir changer de référence
  * Les os sélectionnés (mais non actifs) seront définis comme les os de référence.  
<br/>
* On peut copier un système existant
* On peut copier par mirroir un système existant  
![Copy]({{site.base_url}}/assets/img/AutoRefSpace/system_copy.png)  

### Données dans les systèmes de références

* Label : Le label de la liste déroulante qui sera créée
* Bone : L'os qui pourra changer de référence
* Reference Bones : La liste des os qui serviront de références. Il y a plusieurs manières de les remplir  
  * En sélectionnant tous les os souhaités, puis en cliquant sur 'Fill from Selection'
  * En cliquant sur '+', et en complétant le nom de l'os en bas de la liste, ou en cliquant sur l'icone 'os', qui choisira l'os actif
* Reference Bone Labels : Pour chaque os de référence, on peut choisir un label qui sera affiché dans la liste déroulante. Par défaut, le label est le nom de l'os.
![System Detail]({{site.base_url}}/assets/img/AutoRefSpace/system_detail_2.png)  

### Activer un système

![Activate]({{site.base_url}}/assets/img/AutoRefSpace/active_autoref.png)  
<br/>
Cela va activer le système correspondant. Une liste déroulante est maintenant disponible (avec les labels remplis précédemment)
<br/>
![Choose]({{site.base_url}}/assets/img/AutoRefSpace/choose_ref.png)  
<br/>
On peut maintenant changer l'espace de référence pour l'os. Il faut cliquer de nouveau sur 'activate' pour désactiver le changement d'espace de référence, et pouvoir y faire des modifications.  
**Ce mode est utilisé uniquement pour tester le système. Il ne faut pas insérer des images clés (keyframes) sur la liste déroulante.**  
Il faut utiliser 'Generation' pour continuer le process, et pouvoir insérer des images clés.  

### Génération

![Generate]({{site.base_url}}/assets/img/AutoRefSpace/generate.png)  
<br/>
Cliquer sur 'Generate' pour créer un nouveau *panel* avec des listes déroulantes pour tous les sytèmes (et pas uniquement le système actif comme c'est le cas avec l'outil 'Activate').  
Les listes déroulantes affichées correspondent uniquement aux os sélectionnés.  
<br/>
![choose_]({{site.base_url}}/assets/img/AutoRefSpace/generated_ref_choose.png)  
<br/>
![chooses_]({{site.base_url}}/assets/img/AutoRefSpace/generated_ref_chooses.png)  
<br/>
On peut choisir où le *panel* sera affiché (barre *Tool* ou *Property* de la vue 3D).  
![view_location]({{site.base_url}}/assets/img/AutoRefSpace/view_location.png)  
<br/>
*Si les données ne sont pas remplies, les données des préférences de l'Addon seront utilisées*  
<br/>
Une fois générés, les systèmes de référence ne peuvent plus être modifiables. Il faut cliquer sur 'update' pour pouvoir les modifier, et cliquer sur 'Generate' de nouveau pour continuer à les utiliser.  
<br/>
![update]({{site.base_url}}/assets/img/AutoRefSpace/update.png)  
<br/>
**Une fois généré, cet Addon n'est plus utile, et vous pouvez utiliser les changements d'espace de référence sur toutes les installations de Blender, sans avoir besoin d'installer/de partager cet Addon avec vos fichier .blend.**

[1]: {{site.base_url}}/AddonInstallation-fr/
