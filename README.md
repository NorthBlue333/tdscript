# tdscript
*Ce projet a été réalisé en suivant les consignes du TD scripting [ici](https://gitlab.com/alsim/linux1/blob/master/TD-scripting.md)*
Tous les scripts sont en bash
N'oubliez pas de chmod +x les fichiers pour les rendre exécutables !

## moreorless
C'est le jeu du plus ou moins : le script génère un nombre aléatoire entre 0 et 1000 à chaque exécution. Ensuite, tant que le nombre n'est pas trouvé, le joueur doit entrer un nombre, et le script répondra soit plus, soit moins.
Il a été testé ainsi :
* Caractères autres que des nombres
* Nombre supérieur
* Nombre inférieur

*Pour exécuter : `./moreorless`*

## savetool
Ce script est un utilitaire de sauvegarde en .tar. Lorsqu'il est lancé, il vérifie le jour de la semaine : si c'est un autre jour que vendredi, il exécute une sauvegarde incrémentale, sinon, il fait une sauvegarde entière. Pour la sauvegarde incrémentale, il est possible de choisir si l'on veut sauvegarder tous les nouveaux fichiers ou les fichiers modifiés dans les dernières 24h.
Il a été testé ainsi :
* Dossier backups inexistant
* Autre jour que vendredi mais pas de backup de vendredi dernier
* Vendredi
* Autre jour que vendredi
* Pas d'entrée
* Mauvais path
* Mauvais numéro d'option

Il ne marche qu'avec la langue du système en anglais ou en français.

*Pour exécuter : `./savetoool "pathtosave"`*

## youtube-dl
Ce script est un utilitaire de téléchargement de fichier son de vidéo (youtube et autres plateformes). Il téléchargement automatiquement le meilleur format audio, le met dans le dossier youtube-dl-musics du dossier Home de l'utilisateur et retire l'url de son nom.
Il a été testé ainsi :
* Pas d'entrée
* Mauvaise url
* Dossier youtube-dl-musics inexistant

*Pour exécuter : `./youtube-dl url`*
