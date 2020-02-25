---
layout: tool
title: ExtraGroups
lang: fr
ref: ExtraGroups
permalink: /fr/tools/ExtraGroups/
redirect_from:
  - /tools/ExtraGroups-fr/
cat: animation
sort_nb: 1
stable_version: v1.1.0
stable_status: Publié le 18 janvier 2020
dev_version: N/A
dev_status: Pas de développement en cours
description: Gérez vos os facilement !
img: ExtraGroups.png
getit_url:
  - label: Gumroad
    url: https://gumroad.com/l/ExtraGroups
  - label: BlenderMarket
    url: https://blendermarket.com/products/extragroups
display_url: true
---

## Pour démarrer
Si vous ne savez pas installer un Addon, suivez la [procédure suivante][1].  

## Présentation  

Cet addon permet de gérer des groupes d'os, pendant l'animation (en mode _Pose_).  
On peut gérer les groupes d'os (en créer, supprimer, trier, ajouter / supprimer des os dans les groupes).  
Pour chaque groupe, on peut réaliser des actions (_opérateurs_). On peut choisir quels sont les opérateurs qui sont affichés, et dans quel ordre.  

![][22]

{% include youtube.html id='Ljteyl8XUFM' %}

## Démarrer avec ExtraGroups

![][4]

Si vous êtes nouveau dans l'utilisation de cet addon, clickez sur "Create from scratch" pour initialiser les données par défault.  
Si vous savez ce que vous faites, allez voir du côté des imports/exports, dans ce manuel.  

## Gérer vos groupes

![][3]

On peut gérer les groupes que lorsque l'addon est en mode _Edit_ :

![][5]

# Créer des groupes

Quand on créé un groupe, tous les os sélectionnés dont automatiquement ajoutés dans ce nouveau groupe. A noter qu'un os peut appartenir à plusieurs groupes.  
Pour chaque groupe, on peut définir quel est l'os principal de ce groupe. Quand on créé un groupe, cet os principal est l'os actif de la sélection.  

# Supprimer des groupes

Le groupe est supprimé. Les propriétés des os qui peuvent avoir été changées par les opérateurs ne sont pas restorées.  

# Mise à jour des groupes

*  Ajouter un os au groupe courant : Tous les os sélectionnés sont ajoutés au groupe actif.  
*  Supprimer des os du groupe courant : Tous les os sélectionnés sont supprimés du groupe actif.  

# Copier un groupe (par miroir ou non)

![][6]

*  Copier un groupe
Le groupe est copié : liste des os, et toutes les propriétés correspondantes.  
*  Copier un groupe par miroir
Le groupe est copié, mais le nouveau groupe contient tous les os miroir du groupe d'origine (suffixe _.L_ changé en suffixe _.R_ par exemple). Les os qui n'ont pas de suffixe définissant leur côté (droite/gauche), sont gardés tels quels dans le nouveau groupe. Si le nom du groupe contient un suffixe, alors le nom du nouveau groupe sera modifié pour en tenir compte.  

# Le groupe 'current selection'

Actif par défaut, ce groupe est un groupe spécial, qui contient toujours la liste des os sélectionnés dans la vue 3D. On ne peut donc pas ajouter ou supprimer des os de ce groupe.  
Certains opérateurs ne sont pas disponible pour ce groupe spécial.  

Si vous supprimez ce groupe, un nouveau bouton est disponible pour l'ajouter de nouveau.  

![][7]
<br/>
<br/>
## Gérer vos opérateurs

![][8]

Les opérateurs sont es actions que l'on peut réaliser sur les os de vos groupes (même si les os de ce groupe ne sont pas sélectionnés dans la vue 3D).  
On peut gérer les opérateurs uniquement en mode edit de l'addon.  

# Affiché ou non ?

On peut décider d'afficher ou non l'opérateur. N'affichez pas les outils dont vous n'avez pas besoin !  
Par défaut, _Sélection_ et _Visibilité_ sont les 2 opérateurs affichés.

# Trier les opérateurs

On peut trier les opérateurs dans la liste. Cet ordre sera utilisé dans le panneau et la popup :)

# Ajouter / supprimer des opérateurs

Ajouter des opérateurs est seulement disponible en mode _développeur_ (voir dans les préférences de l'addon).  
Seuls les opérateurs ajoutés par l'utilisateur (donc en mode développeur) peuvent être supprimés.  

# Changer les icônes

On peut changer les icônes pour chaque opérateur.  
Pour les opérateurs qui réalisent une action, il y a 1 icônes. Pour les opérateurs de type _on/off_, il y a 2 icônes.  

On peut changer les icônes directement en tapant leur nom (si vous le connaissez), ou bien en la sélectionnant dans la liste (disponible en dépliant le petit triangle).  

![][9]

# Détail des opérateurs

Certains détail des opérateurs peuvent être affichés:
*  gestion des évènements / modes (voir en dessous)  
*  Si l'opérateur est disponible pour le groupe spécial '_current selection_'
*  Des détails techniques disponibles uniquement en mode développeur.

## Gestion des évènements / mode

![][10]

Pour chaque opérateur, il peut y avoir des comportements différents. Par exemple, pour l'opérateur _Sélection_, on peut vouloir sélectionner uniquement le groupe, ajouter le groupe à la sélection, ou bien sélectionner uniquement le groupe, et cacher tous les os des autres groupes. Ces différents modes sont accessibles avec les touches de modification (Ctrl, Shift, Alt, ...).  

# Activer les évènements

Pour chaque opérateur, on peut décider quels sont les modes/évènements actifs ou non.

# Gérer les raccourcis.

Pour chaque moed, on peut décider quel est la touche modificatrice qui doit être utilisée.  
Si une touche est liée à plusieurs modes différents, alors un message d'avertissement est affiché.  

![][11]

## Liste des opérateurs

Voici la liste de tous les opérateurs disponibles, et les différents modes correspondant :  
Pour la plupart des modes, une version _miroir_ est aussi disponible (ce qui signifie que l'opérateur ne s'applique pas sur le groupe, mais sur sa version miroir).  

# Sélection
*  _Select only
Sélectionne uniquement le groupe (les autres os sont de-sélectionnés).  
*  _Add to selection_
Ajoute les os du groupe à la sélection courante.  
*  _Remove from selection_
Déselectionne les os du groupe.  
* _Select only and hide others_
Sélectionne les os du groupe (les autres os sont de-sélectionnés et rendus non visibles).
* _Select opposite_
De-sélectionne le group, et sélectionne tous les autres os.  


# Mute
* Mute
Met en _mute_ toutes les animations des os du groupe.
* mode solo
Met en _mute_ toutes les animations des os qui ne sont pas dans le groupe.

# Visibilité
* _Toggle visiblity_
Cache les os du groupe s'ils sont visibles, les rend visibles s'ils sont cachés.
* mode solo
Cache les os qui ne sont pas dans le groupe

# Restriction de la sélection
* Toogle
Rend sélectionnable / non sélectionnable les os du groupe
* mode solo
Rend non sélectionnable les os qui ne sont pas dans le groupe.

# Propriétés
Affiche une popup où les propriétés des os peuvent être changées.

# Lock
Bloque les channels des os du groupe (il n'est plus possible d'ajouter alors des _keyframes_)

# Keyframing
* Défaut
Ajoute les keyframes sur les os du groupe, en utilisant le KeyingSet du groupe (voir l'option plus loin). S'il n'y a pas de KeyingSet renseigné dans les options du groupe, un menu est affiché pour choisir quelles keyframes ajouter.  
* Forced menu
Ajoute les keyframes sur les os du groupe, en affichant le menu, même si un keyingset est renseigné pour le groupe (voir options)
* Keying Only
Ajoute les keframes sur les os du groupe, en utilisant le KeyingSet du groupe (voir l'option). S'il n'y a pas de KeyingSet renseigné dans les options du groupe, aucune keyframe n'est ajoutée.  

# Motion Path
* Add/Remove motion path
Ajoute / Enlève le _motion path_ sur les os du groupe.
* update motion path
Met à jour le _motion path_ des os du groupe.

## Options

![][12]

# Gestion des KeyingSet

![][13]

On peut choisir de rattacher un keyingset existant à un groupe. Si la gestion des keyingsets est actif, et qu'un keyingset est renseigné:
*  En utilisant l'opérateur _sélection_, le KeyingSet actif de la scène est automatiquement changé.
*  En utilisant l'opérateur _Keyframing_, le KeyingSet sera utilisé pour ajouter des keyframes (sauf si on utilise le mode _Forced Menu_).

# Gestion des transformations Gizmo
![][14]

On peut choisir le gizmo à utiliser, ainsi que l'espace d'évaluation des axes. Cela sera changé automatiquement quand on utilise l'opérateur _Sélection_.

# Couleur des groupes
![][15]

On peut choisir d'utiliser une couleur pour chaque groupe (pour éviter d'avoir à lire le nom du groupe ;-) )
La couleur est modifiable en mode edit.  

# Multitype
![][16] ![][17]  
On peut couper les groupes en plusieurs sous-groupe. Pour chacun des sous-groupe, on peut avoir une liste différente d'opérateurs.  

Pour la popup, par défaut la liste des sous-groupe n'est pas afichée, mais elle est accessbile via le bouton correspondant.

![][18] ![][19]

# Nom clickable

Quand on active cette fonctionnalité, le nom du groupe (dans la liste) est clickable. On peut choisir l'opérateur qui sera exécuté. Deux solutions :  
*  On décide quel mode est utilisé quand on clique. (et aucune touche de modification n'est active)  
  ![][20]
*  On choisit d'utiliser les mêmes évènements que l'opérateur (accessible avec l'icône).  
  ![][21]

## Import / Export

Import / Export est accessible quand la checkbox est cochée.  
![][23]

# Exporter dans un fichier
On peut exporter les données dans un fichier texte. La plupart des données de l'addon sont exportées :
*  Les groupes, les os correspondant
*  Les opérateurs (le tri et lesquels sont affichés)
*  La plupart des options (couleur, gizmo, keyingset, nom clickable)

# Importer depuis _Bone Groups_
Si des _Bone Groups_ (fonctionnalité de Blender) sont définis, on peut automatiquement les convertir en groupes d'os.

#	Importer depuis _Selection Sets_
Si des groupes sont définis dans _Selection Sets_ (un addon de Blender), on peut automatiquement les convertir en groupes d'os.

# Importer depuis les KeyingSets
Si des KeyingSets sont définis sur le rig, on peut automatiquement les convertir en groupes d'os.

# Importer depuis un fichier
On peut importer les données depuis un fichier, généré en utilisant l'export dans un fichier. (Il vaut mieux utiliser la même version de l'addon).

## Utiliser l'addon avec des armatures _linkées_
On peut utiliser ExtraGroups avec les rigs _linkés_. Disons qu'on a un fichier _Rig_, dans lequel se trouve l'armature, et un fichier _animation_, où l'armature est ajouté par _link_, et où l'animation est faite. Il y a 2 étapes :  
*  Créer les données de l'addon dans le fichier _Rig_ (créer les groupes, gérer les opérateurs, les évènements)
*  Sur le fichier _animation_, quand on active l'addon sur un rig ajouté en mode _link_, les données sont automatiquement importées depuis le fichier _Rig_ vers le fichier _animation_.
*  Si on veut changer des données (opérateurs, groupes, os dans les groupes, ...), on peut le faire directement dans le fichier _animation_, si on a besoin de ces modifications uniquement dans ce fichier animation.
*  Si l'armature est utilisée dans plusieurs fichiers d'animation, il faut faire les modifications dans le fichier _Rig_. Dans le fichier _animation_, en mode _edit_, il y a un noueau outil qui permet de réimporter les données (avec les modifications) depuis le fichier _Rig_ vers le fichier _animation_.
  ![][24]

## Mode développeur

Le mode développeur de l'addon ExtraGroups, est utilisé pour créer ses propres opérateurs. Je ne suis pas sûr que cette fonctionnalité soit complètement stable. Je ne vais pas la documenter pour le moment, en espérant que ça vous insite à ne pas l'utiliser ;-)

## Préférences de l'addon

![][25]

# Display
On peut choisir d'afficher ou non la popup. Et de choisir le raccourci.  
On peut choisir dans quel onglet se trouve l'addon.

# Mode développeur
Si vous souhaitez vraiment l'utiliser, contactez-moi que je vous explique !

# Zone de Danger
Si quelque chose se passe mal, il est possible de supprimer toutes les données relatives à ExtraGroups dans le fichier.

## Mise à jour de l'addon.

Il n'a pas de mise à jour automatique sur cet addon (pour le moment). On peut donc le mettre à jour en suivant les étapes suivantes :
*  desactiver l'addon
*  le désinstaller
*  installer la nouvelle version
*  activer la nouvelle version

Pour certaines mises à jour, certaines données interne de l'addon doivent être mises à jour. Ce qui signifie que cela doit être fait avant d'utiliser la nouvelle version. Pas de panique, ce n'ai pas compliqué !

# Pour les rigs locaux
Pas de système de _link_ Le cas le plus simple :)
A la place des panneaux habituels, il y a un bouton qui demande de mettre à jour les données. Cliquez, et c'est fait :)

![][26]

# Pour les rigs _linkés_
Il faut mettre à jour __en premier__ le fichier _Rig_. Ensuite, on peut mettre à jour le fichier _animation_.

![][27]

Donc, les étapes sont :
*  Mettre à jour l'addon
*  Fermer le fichier _animation_
*  Ouvrir le fichier '_Rig_'
*  Mettre à jour les données de l'addon en cliquant sur le bouton qui demande la mise à jour
*  Sauvegarder le fichier _Rig_, et le fermer
*  Ouvrir le fichier _animation_
*  Cette fois-ce, on peut utiliser _Reload from library_ pour mettre à jour les données depuis le fichier _Rig_ vers le fichier _animation_
*  Sauvegarder le fichier !

## Comment faire un rapport de bug ou demander une nouvelle fonctionnalité ?
On peut le faire [ici][2]

## Historique des versions
*  __v1.0.0__, 20 mai 2017 : premier version publiée
*  __v1.0.1__, 20 décembre 2017 :  
    *  Mute & Lock: bug quand une action existe, mais sans keyframes
* __v1.1.0__, 18 janvier 2020
    * Mise à jour pour Blender 2.80+


[1]: {{site.base_url}}/en/AddonInstallation/
[2]: https://github.com/julienduroure/BleRiFa/issues/
[3]: {{site.base_url}}/assets/img/ExtraGroups/manage_groups.png
[4]: {{site.base_url}}/assets/img/ExtraGroups/init.png
[5]: {{site.base_url}}/assets/img/ExtraGroups/edit_mode.png
[6]: {{site.base_url}}/assets/img/ExtraGroups/copy_groups.png
[7]: {{site.base_url}}/assets/img/ExtraGroups/current_selection.png
[8]: {{site.base_url}}/assets/img/ExtraGroups/manage_operator.png
[9]: {{site.base_url}}/assets/img/ExtraGroups/icon_picking.png
[10]: {{site.base_url}}/assets/img/ExtraGroups/manage_event.png
[11]: {{site.base_url}}/assets/img/ExtraGroups/event_warning.png
[12]: {{site.base_url}}/assets/img/ExtraGroups/options.png
[13]: {{site.base_url}}/assets/img/ExtraGroups/keyingset.png
[14]: {{site.base_url}}/assets/img/ExtraGroups/gizmo.png
[15]: {{site.base_url}}/assets/img/ExtraGroups/colorlabel.png
[16]: {{site.base_url}}/assets/img/ExtraGroups/grouptype_legs.png
[17]: {{site.base_url}}/assets/img/ExtraGroups/grouptype_arms.png
[18]: {{site.base_url}}/assets/img/ExtraGroups/grouptype_popup_1.png
[19]: {{site.base_url}}/assets/img/ExtraGroups/grouptype_popup_2.png
[20]: {{site.base_url}}/assets/img/ExtraGroups/name_clickable_1.png
[21]: {{site.base_url}}/assets/img/ExtraGroups/name_clickable_2.png
[22]: {{site.base_url}}/assets/img/ExtraGroups/popup.png
[23]: {{site.base_url}}/assets/img/ExtraGroups/import_export.png
[24]: {{site.base_url}}/assets/img/ExtraGroups/linked_reload.png
[25]: {{site.base_url}}/assets/img/ExtraGroups/addonpreferences.png
[26]: {{site.base_url}}/assets/img/ExtraGroups/update_addon.png
[27]: {{site.base_url}}/assets/img/ExtraGroups/reload_library_update.png
