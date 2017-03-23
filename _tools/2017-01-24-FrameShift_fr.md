---
layout: tool
title: FrameShift
lang: fr
ref: FrameShift
permalink: /fr/tools/FrameShift/
redirect_from:
  - /tools/FrameShift-fr/
cat: animation
sort_nb: 4
stable_version: N/A
stable_status: Pas encore publié
dev_version: 0.0.1
dev_status: En développement
description: Gérer le timing en décallant les keyframes
img: FrameShift.png
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

_FrameShift_ est utilisé pour déplacer/décaller rapidement les _keyframes_ (en avant ou en arrière)

{% include html5video.html id="FrameShift_1.ogv" %}

# Comment ça marche ?

Pour le moment, cet addon fonctionne uniquement en mode _Pose_ (donc uniquement pour les _Rigs_)

## Où ça ?

Il peut être utilisé :

* Dans le  _DopeSheet_
* Dans le _GraphEditor_
* Dans la  _TimeLine_
*	Dans la vue 3D

## Comment ?
Avec le raccourci _Shift+Q_, cela va avancer toutes les _keyframes_ qui sont après la _frame_ courante.  
En pressant _Alt+Shift+Q_, cela va reculer toutes les _keyframes_ qui sont après la _frame_ courante. Si on recule trop les _keyframes_, l'addon ne supprimera pas les images clefs, ni ne crééra de supperposition.

## Combien de _Frames_ ?
Le décallage est défini dans le paramètre de l'opérateur. Par défaut, la valeur est 1.  
Quand on le change (après avoir apuyé sur _Shift+Q_ ou _Alt+Shift+Q), le nombre de _frames_ est sauvegardé, et cette valeur sera utilisé au prochain appel. On peut aussi modidier le sens (en avant / en arrière)

![OpsParameter]({{site.base_url}}/assets/img/FrameShift/OpsParameters.png)

# Préférences de l'addon
![AddonPref]({{site.base_url}}/assets/img/FrameShift/AddonPref.png)
* On peut changer le raccourci  
* On peut choisir si le décallage est appliqué sur l'ensemble du rig, ou uniquement sur les os sélectionnés  

# Comment rapporter un bug ou demander une nouvelles fonctionnalité ?
Vous pouvez le faire sur le [Tracker][2]

[1]: {{site.base_url}}/fr/AddonInstallation/
[2]: https://github.com/julienduroure/BleRiFa/issues/
