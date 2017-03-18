---
layout: tool
title: FootRollBreak
lang: fr
ref: footrollbreak
permalink: /tools/FootRollBreak-fr/
cat: rigging
sort_nb: 5
stable_version: 1.0.0
stable_status: Publié le 25 mars 2016
dev_version: N/A
dev_status: Pas de développement en cours
description: Améliorez les pieds de vos rigs Rigify
img: FootRollBreak.png
getit_url:
  - label: Blender Market
    url: https://cgcookiemarkets.com/all-products/footrollbreak/
  - label: Gumroad
    url: https://gumroad.com/l/FootRollBreak
display_url: true
---

# Pour démarrer
Si vous ne savez pas installer un Addon, suivez la [procédure suivante][1].  

# FootRollBreak
FootRollBreak est un addon qui améliore les rigs réalisés avec _Rigify_, en rajoutant la possiblité de faire du _FootRollBreak_, c'est à dire d'avoir un mouvement plus naturel en utilisant la fonctionnalité _Foot Roll_ déjà présente dans les rigs.

{% include html5video.html id='FootRollBreak.ogv' %}  

# Démarrage rapide

*  Installer l'addon _FootRollBreak_, et l'activer
*  Selectionner le rig _Rigify_, and aller dans les propriétés de l'armature. Un nouveau panneau est présent :)
*  Patcher le rig (fonctionne avec les deux types _Human_ et _Pitchipoy_)
*  Un nouveau panneau se trouve dans le pannel des propriétés de la vue 3D (N), non loin des autres panneaux liés à _Rigify_.
*  C'est tout :)
*  _FootRollBreak_ reste actif même si vous désinstallez l'addon.

![angles]({{site.base_url}}/assets/img/FootRollBreak/angles.png)

# Comment patcher le rig ?

*  Assurez-vous d'avoir sélectionné un rig _Rigify_ (pas le _metarig_, mais bien le rig réel, après génération)
*  Dans les propriétés de l'armature, un nouveau pannel "Rigify FootRoll Break Patch" est disponible
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/addon_panel.png)  
<br/>
*  Patcher le rig en cliquant sur le bouton "Patch FootRoll Break" (cela fonctionne sur les 2 types de rig _Human_ et _Pitchipoy_)
*  Le bouton est maintenant remplacé par le text "already patched!"
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/already_patched.png)  
<br/>
* Entrez en mode _Edit_ sur l'armature, et ajustez le nouvel os "toe-top" pour définir le centre de rotation au bout des orteils. Retournez en mode _Pose_.  
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/toe-top.png)  
<br/>

# Comment utiliser cette nouvelle fonctionnalité ?

*  FootRoll Break est désactivé par défaut. Si vous essayé d'utiliser le _Foot Roll_, rien ne se passe (ou bien plutôt tout se passe comme d'habitude)
*  Un nouveau _panel_ se trouve dans les propriétés de la vue 3D (N)  
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/ui_panel.png)  
<br/>
*  Activez l'option _FootRollBreak_ (avec la _checkbox_ correspondante)  
![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/footrollbreak_option.png)  
<br/>
*  Essayez de nouveau de faire un _Foot Roll_ :
  *  Arrivé à l'angle défini en paramètre, le pied commence à se soulever, et les orteils à se "déplier"
  *  Arrivé à l'"angle max", défini dans les paramètres, les orteils complètement dépliés.
  *  Dans certains cas (assez rare), le pied aura un mouvement peut naturel. Dans ces cas, vous pouvez modifier le paramètre "corrective angle" afin d'obtenir un meilleur mouvement.
  <br/>
  ![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/bad_motion.png)
  ![Screenshot patch]({{site.base_url}}/assets/img/FootRollBreak/correct_motion.png)

# Restrictions

  La version actuelle de cet addon ne fonctionne qu'avec les bipède Rigify (le métarig par défaut, par exemple), mais ne fonctionne pas avec les rigs ayant 1 seule jamble, ou bien plus de 2 jambes.

# Comment signaler un bug ?
  Vous pouvez utiliser le  [Tracker][2]

# Historique des versions
*  v 1.0.0
  *  Date : 25 Mars 2016
  * Change logs:
    * Version initiale

[1]: {{site.base_url}}/AddonInstallation-fr/
[2]: https://github.com/julienduroure/FootRollBreak/issues/
