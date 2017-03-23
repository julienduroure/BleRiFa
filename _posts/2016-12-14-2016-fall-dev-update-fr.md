---
layout: post
title: "Automne 2016 : Mises à jour"
lang: fr
ref: 2016-fall-update
img: 20161214_dev_update.png
permalink: /fr/:year/:month/2016-mise-a-jour-automne/
redirect_from:
  - /2016/12/14/2016-mise-a-jour-automne/
version: 2
---

Bonjour à tous,
Dans le but de faire ça de manière trimestrielle, voici les nouvelles des mois précédents :)


# Blender Conference
J'ai donné cette année une conférence sur [BleRiFa][1]. Si vous ne l'avez pas vu, allez-donc [lire mon compte rendu, et voir la vidéo][2].

# BoneChainRenamer
J'ai fait quelques mises à jour sur l'outil [BoneChainRenamer][3] :  
Avant les modifications, quand on renommait plusieurs chaines, l'ordre des chaînes était alphabétique. On peut maintenant choisir l'odre des chaines :   

*  Par distance
*  Par position (X/Y/Z and X/Y/Z inversé)

La doc doit encore être mise à jour

# ExtraGroups

*  Il y a un nouveau _panel_, à partir duquel on peut importer :  
	*  Depuis les _Bone Groups_
	*  Depuis les _Keying Sets_
	*  Depuis les _Selection Sets_

*  Ces 3 importeurs sont aussi accessibles depuis les préférences utilisateurs
*  La case à cocher pour passer en mode _Edit_ est accessible directement depuis l'interface, pas uniquement depuis les préférences.
*  Le groupe de sélection courante ('_Current Selection_') est disponible par défaut
*  Quand l'utilisateur change le _tab_ dans lequel l'addon est affiché, et si l'addon est actif dans les préférences utilisateurs, l'Addon reste dans ce _tab_ à l'ouverture de Blender
*  Et plein de corrections de bugs bien sûr !
*  Partie développement : modification du chargement des modules, on peut maintenant utiliser F8 pour recharger l'Addon
*  D'autres fonctionnalités sont en cours de développement, mais instable pour le moment. Je présenterai ça au cours de la mise à jour de cet hiver ;-)

La doc doit encore être mise à jour

# AutoSnap

*  Partie développement : modification du chargement des modules, on peut maintenant utiliser F8 pour recharger l'Addon

# AutoRefSpace

*  Partie développement : modification du chargement des modules, on peut maintenant utiliser F8 pour recharger l'Addon

# Website
Il n'y a pas eu énormément de mise à jour du site ces derniers mois ... mais j'ai travaillé sur une toute [nouvelle version de mon site web][4]. Cette nouvelle version est aussi basée sur [jekyll][5].
La plupart des améliorations faite sur [mon site][4] seront reportées sur [BleRiFa][1] dans les prochains mois.

[1]: http://BleRiFa.com
[2]: http://BleRiFa.com/fr/2016/11/bcon16-report/
[3]: http://BleRiFa.com/fr/tools/BoneChainRenamer/
[4]: http://julienduroure.com
[5]: https://jekyllrb.com/
