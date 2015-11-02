---
language: Français
currentMenu: theme
subTitle: Créer un nouveau thème
---

# Créer un nouveau thème

Les thèmes sont créés en utilisant le moteur de templates [Twig](http://twig.sensiolabs.org/). Les fichiers se trouvent dans des répertoires différents selon que vous utilisiez la version 1 ou la version 2 :

* Dans la version 1, vous les trouverez dans le répertoire `themes/`.
* A partir de la version 2, ils sont dans `src/Wallabag/CoreBundle/Resources/views/themes/`. Ils y sont groupés par catégorie. Les composants de base (imgs, js, css, fonts) sont dans le sous-répertoire `public/`.

Tous les fichiers de templates étendent un fichier unique nommé `layout.html.twig`.
