---
layout: tool
title: "Bone Picker"
lang: fr
ref: BonePicker
permalink: /fr/tools/BonePicker/
cat: rigging
sort_nb: 4
stable_version: 0.0.1 (version alpha)
stable_status: Version alpha publique
dev_version: 0.0.2
dev_status: En développement
description: Sélectionnez les os superposés
img: BonePicker.png
getit_url:
  - label: Gumroad
    url: https://gumroad.com/l/BonePicker
display_url: true
---

# Pour démarrer
Si vous ne savez pas installer un Addon, suivez la [procédure suivante][1].

# Aperçu

Cet addon est utilisé pour sélectionner facilement les os superposés.  
On peut également connaitre les os superposés mais non sélectionnable (car invisible ou sur un autre _layer_).

![]({{site.base_url}}/assets/img/BonePicker/popup.png)

{% include html5video.html id="BonePicker.ogv" %}

# Comment ça marche ?

A l'affichage de la _popup_ (activée à l'aide du raccourci clavier défini dans les paramètres de l'addon), on peut :  

*  sélectionner un os avec le click souris
*  Ajouter à la sélection avec Shift+click
*  Dé-sélectionner en re-cliquant sur un os

On peut voir :  
*  les os qui sont actuellement sélectionnés
*  l'os actif

On peut également (os non sélectionnable) :  

*  Voir les os superposés qui sont invisible
*  Voir les os superposés qui sont sur un autre _layer_

# Options

Le raccourci clavier utilisé peut être modifié dans les réglages de l'addon.  
On peut également régler la sensibilité pour la détection des os superposés.

![]({{site.base_url}}/assets/img/BonePicker/UserPref.png)

# Comment rapporter un bug ou demander une nouvelles fonctionnalité ?
Vous pouvez le faire sur le [Tracker][2]

[1]: {{site.base_url}}/fr/AddonInstallation/
[2]: https://github.com/julienduroure/BleRiFa/issues/
