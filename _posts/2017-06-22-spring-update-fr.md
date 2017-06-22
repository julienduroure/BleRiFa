---
layout: post
title: "BleRiFa : Mises à jour printemps 2017"
lang: fr
ref: 2017-spring-update
img: 20161214_dev_update.png
permalink: /fr/:year/:month/2017-mises-a-jour-printemps/
version: 1
---

Quoi de neuf sur BleRiFa ?

# [ExtraGroups][1]

![][15]

La version v1.0 de ExtraGroups est sortie !
La [documentation][1] est maintenant complète, et l'addon est disponible sur le [BlenderMarket][2] and [Gumroad][3]

*  On peut maintenant afficher l'outil sous forme de popup
*  Copie des groupes / copie mirroir
*  Nouvel opérateur : _Motion Path_
*  Selection & visibilité sont maintenant initialisé par défaut
*  Les opérateur sont maintenant toujours affichés dans le même ordre
*  On peut cliquer sur le nom du groupe
*  Système d'évènements :
	*  Nouveau mode pour la sélection : _Select and hide others_
	*  Nouveau mode pour la sélection : _Select opposite_
	*  Affichage d'un label au lieu du mode directement
	*  Possibilité d'activer/désactiver les évènements pour chaque opérateur
	*  Solo mode pour l'opérateur _Lock_
	*  Evènement mirroir pour tous les opérateurs
*  Gestion des manipulateurs pour l'opérateur sélection (Gizmo / axes)
*  Gestion de l'os actif dans chaque groupe
*  Import / Export :
	*  Couleur / gizmo / axes / os actif
	*  Import/Export des opérateurs affichés
	*  Import/Export de l'ordre des opérateurs
*  Gestion de la couleur des groupes directement dans l'interface, modifiable uniquement en mode edit
*  Meilleure interface pour les préférences de l'addon, et les options
*  Mode solo non bloquand
*  Et bien sûr des corrections de bugs ici ou là

# [AutoRefSpace][4]
*  Implémentation d'un nouveau système pour éviter des soucis de calculs matriciels (quand on utilise _Selection to Cursor_). L'interface utilisateur n'est pas modifiée, mais tout ce qu'il y a derrière a été recodé. Il y a encore du travail avant de pouvoir faire une version béta privée.

{% include html5video.html id="AutoRefSpace_1.ogv" %}

# [PanelMaker][5]
*  Il est maintenant possible de créer des boutons pour gérer toutes les propriétés de tous les objets de la scène.

{% include html5video.html id="PanelMaker_2.ogv" %}

# [FrameShift][10]
*  J'ai rajouté un petit outil pour [décaller les _frames_][10].

{% include html5video.html id="FrameShift_1.ogv" %}

# [FootRollBreak][6]
*  FootRollBreak est maintenant disponible sur [Gumroad][11] également.
*  Mise à jour de la [documentation][6] pour expliquer comment faire fonctionner les rigs _linkés_

# [Mass KeyingSet][7]
*  Cet addon est maitenant disponible sur le [BlenderMarket][8] et [Gumroad][9]

# Sur le site de BleRiFa
*  Quelques mises à jour de layout par ci par là
*  Les outils sont maintenant affichés sur la page d'accueil sous forme de tuiles
*  Grosse mise à jour de tous les liens permanents.
*  Un article sur la sortie de la [version v1.0 de ExtraGroups][12]


# Sur le site _julienduroure.com_
*  [10 choses à vérifier sur un Rig][13]
*  [Tuto animation météo][14]

[1]: {{site.base_url}}/fr/tools/ExtraGroups/
[2]: https://blendermarket.com/products/extragroups
[3]: https://gumroad.com/l/ExtraGroups
[4]: {{site.base_url}}/fr/tools/AutoRefSpace/
[5]: {{site.base_url}}/fr/tools/PanelMaker/
[6]: {{site.base_url}}/fr/tools/FootRollBreak/
[7]: {{site.base_url}}/fr/tools/MassKeyingSets/
[8]: https://blendermarket.com/products/mass-keyingsets
[9]: https://gumroad.com/l/SRqtl
[10]: {{site.base_url}}/fr/tools/FrameShift/
[11]: https://gumroad.com/l/FootRollBreak
[12]: {{site.base_url}}/fr/2017/05/ExtraGroups-V1-release/
[13]: http://julienduroure.com/fr/2017/05/10-choses-a-verifier-sur-un-rig/
[14]: http://julienduroure.com/fr/2017/06/tuto-anim-meteo/
[15]: {{site.base_url}}/assets/img/ExtraGroups/popup.png
