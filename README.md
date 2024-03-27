# guide-mint

Le but de ce tuto est de vous aider à installer et configurer une Linux Mint afin de pouvoir l'utiliser pour du multimédia / Gaming.

En construction... Sujets à aborder :

## 1. Comment procéder à l'installation

Si besoin d'aide pour réaliser une clé bootable depuis Windows, vous pouvez consulter [cette page](https://github.com/Gaming-Linux-FR/glf-astuces/blob/main/README.md#comment-cr%C3%A9er-une-cl%C3%A9-bootable-depuis-windows).

A compléter

## 2. Mettre à jour son système et chosir ses mirroirs

A compléter

## 3. Modifier le vm.max_map_count (à faire jusqu'à la version 22 de Linux Mint)

A compléter

## 4. Installer les logiciels

Une logithèque est mise à disposition sur Linux Mint pour installer vos applications. Pour accéder à celle-ci, il vous faut aller dans dans le menu des applications (1) et cliquer sur cette icône (2) :

![LM-acces-logitheque](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/ad2a9e25-274a-48fb-983d-f4e8d470ea7c)

Une fois ouverte, cela ressemblera à ceci :

![LM-logitheque-accueil](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/84b0a680-438e-455d-9951-7647504b6b55)

A partir de là, vous pouvez parcourir la liste des applications proposées ou faire une recherche ciblée. Par exemple, pour la partie gaming, vous aurez besoin d'installer Steam, il suffit donc de rechercher celui-ci :

![LM-logitheque-steam](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/35f8db07-d685-44cd-b927-f59f5cf0816b)

Ici, on peut voir plusieurs résultats et c'est les deux premiers qui vont nous intéresser. Le premier est un paquet système, c'est à dire un paquet dans les dépôts de la distribution et donc validé par celle-ci. Le second avec la mention "flatpak" est un paquet universel venant de flathub.

Les deux paquets vont fonctionner mais il est bon à noter de façons générales les points suivants :
- Les paquets systèmes sont souvent plus vieux (mais certains comme steam ont un système de mise à jour indépendant) et fonctionnent avec ce qui est installé sur le système ou fait ajouter des composants à votre système pour tourner.
- Les paquets flatpak tournent avec leur propre environnement et embarque tout avec eux (ce qui fait que leur taille est plus importante) et son fourni dans la dernière version stable publiée et fonctionnent de la même manière avec tous les distributions. Ils ont aussi l'avantage de faire venir la dernière version de Mesa, ce qui est intéressant quand on utilise de l'Intel / AMD. En revanche, ils ont un accès limité au système, ce qui sécurise d'un côté mais rend certaines actions plus compliquées, notamment l'accès aux disques secondaires (voir [page suivante](https://github.com/Gaming-Linux-FR/glf-astuces?tab=readme-ov-file#acc%C3%A8s-%C3%A0-un-second-disque-sur-steam-flatpak)).

## 5. Désactivation de la composition des fenêtres pour de meilleures performance en jeu

A compléter
