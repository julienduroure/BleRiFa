---
layout: tool
title: Mass KeyingSets
lang: fr
ref: masskeyingsets
permalink: /fr/tools/MassKeyingSets/
redirect_from:
  - /tools/MassKeyingSets-fr/
cat: animation
sort_nb: 2
stable_version: 0.2.1
stable_status: Version disponible publiquement
dev_version: N/A
dev_status: N/A
description: Création de KeyingSets en masse
img: MassKeyingSets.png
getit_url:
- label: Blender Market
  url: https://blendermarket.com/products/mass-keyingsets
- label: Gumroad
  url: https://gumroad.com/l/SRqtl
- label: Github
  url: https://github.com/julienduroure/MassKeyingSets
display_url: true
---

## Pour démarrer
Si vous ne savez pas installer un Addon, suivez la [procédure suivante][1].  

## Aperçu

![Panel]({{site.base_url}}/assets/img/MassKeyingSets/panel.png)  
<br/>
Un nouveau panneau est disponible dans les propriétés de la scene (avec les autres panneaux relatifs aux *KeyingSet*).  
Ce panneau est visible uniquement :  
* En mode *pose* sur une armature, quand au moins un os est sélectionné  
* En mode *object*, quand au moins un objet est sélectionné  

Quand on clique sur le premier bouton, une popup permet de choisir quelles sont les informations que l'on veut stocker dans le *KeyingSet*.  
Il y a 2 popup différentes, suivant que l'on soit en mode *pose* ou *object*.    

![Bones]({{site.base_url}}/assets/img/MassKeyingSets/popup_bones.png)  
<br/>
![Objects]({{site.base_url}}/assets/img/MassKeyingSets/popup_objects.png)  

Quand on cliques sur le 2ème bouton, le _KeyingSet_ est créé à partir de toutes les propriétés ayant déjà une animation dans la scène (position, rotation, mise à l'échelle pour les objects, mais également propriétés personnalisées)

## Options

# Mise à jour  
Si l'option est coché, le _KeyingSet_ présent dans le _nom_ sera mis à jour (au lieu de créer un nouveau _KeyingSet_)

# Nom  

Nom du *KeyingSet* qui va être créé.

# Location, Rotation, Scale

Information à prendre en compte dans le *KeyingSet* : Position, Rotation, Mise à l'échelle.

# Bone Custom Properties

Toutes les propriétés personnalisées de tous les os sélectionnés seront rajoutées dans le *KeyingSet*

# Object Custom Properties

Toutes les propriétés personnalisées de tous les objects sélectionnés seront rajoutées dans le *KeyingSet* (au niveau objet)

# Object Data Custom Properties

Toutes les propriétés personnalisées de tous les *data* des objects sélectionnés seront rajoutées dans le *KeyingSet* :  
Au niveau *Mesh* pour un objet avec maillage, au niveau *Curve* pour une courbe, etc...

## Comment rapporter un bug ou demander une nouvelles fonctionnalité ?
Vous pouvez le faire sur le [Tracker][2]

## Historique des versions
*  __v0.1.0__, 9 août 2016: Version initiale
*  __v0.2.0__, 22 septembre 2018:  
    *  Bugs corrigés:
      *  Les mises à l'échelle _lockés_ sont maintenant pris en compte correctement
    *  Nouvelles fonctionnalités:
      *  Un _KeyingSet_ peut maintenant être mis à jour
      *  Création de _KeyingSet_ depuis les propriétés déjà animées
*  __v0.2.1__, 1 september 2019 :
    * Mise à jour pour v2.8x

[1]: {{site.base_url}}/fr/AddonInstallation/
[2]: https://github.com/julienduroure/MassKzeyingSets/issues/
