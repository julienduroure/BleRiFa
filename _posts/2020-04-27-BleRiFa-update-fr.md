---
layout: post
title: "BleRiFa: Next"
lang: fr
ref: blerifa_next
img: 20161214_dev_update.png
permalink: /fr/:year/:month/blerifa-next/
version: 1
---

Bonjour à tous,

Comme vous avez dû vous en rendre compte, cela fait longtemps que je n'ai pas posté de nouvelles ici.
La version 2.80 est sortie l'été dernier, et depuis, le seul travail réalisé est la conversion du code vers la version 2.80+ des outils suivants:

* [ExtraGroups][1]
* [BoneChainRenamer][2]
* [MassKeyingSets][3]
* [PanelMaker][4]

Les outils suivants ne seront pas portés sur la version 2.80+ :

* [SwitchAnimView][5], car maintenant cette fonctionnalité est inclue de base dans Blender (mais le [repo][15] est là quand même)
* [FootRollBreak][6], car Rigify a beaucoup évolué depuis, et le code n'est plus vraiment utilisable (mais le [repo][14] est là si vous le voulez)

Ainsi va la vie, le temps me manque pour développer tous ces outils. C'est pourquoi j'ai décidé de mettre le code à disposition de qui le veut ! Ça se trouve par ici :

* [ExtraGroups][7]
* [BoneChainRenamer][8]
* [MassKeyingSets][9]
* [PanelMaker][10]

Et en bonus, deux codes qui me sont demandés régulièrement. La migration sur la version 2.80+ n'est pas faites, mais le code étant disponible, j'espère que quelqu'un réalisera le travail !

* [AutoSnap][11] ([documentation][12] et [repo][11])
* [AutoRefSpace][13] ([documentation][16] et [repo][13])

Bon vent à tout ce code ! N'hésitez pas à forker, et à commenter si vous êtes content que je mette ce code à disposition !


[1]: {{site.base_url}}/fr/tools/MassKeyingSets/
[2]: {{site.base_url}}/fr/tools/BoneChainRenamer/
[3]: {{site.base_url}}/fr/tools/MassKeyingSets/
[4]: {{site.base_url}}/fr/tools/PanelMaker/
[5]: {{site.base_url}}/fr/tools/SwitchAnimView/
[6]: {{site.base_url}}/fr/tools/FootRollBreak/
[7]: https://github.com/julienduroure/ExtraGroups
[8]: https://github.com/julienduroure/BoneChainRenamer
[9]: https://github.com/julienduroure/MassKeyingSets
[10]: https://github.com/julienduroure/PanelMaker
[11]: https://github.com/julienduroure/AutoSnap
[12]: {{site.base_url}}/fr/tools/AutoSnap/
[13]: https://github.com/julienduroure/AutoRefSpace
[14]: https://github.com/julienduroure/FootRollBreak
[15]: https://github.com/julienduroure/SwitchAnimView
[16]: {{site.base_url}}/fr/tools/AutoRefSpace/
