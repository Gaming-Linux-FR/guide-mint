# guide-mint

Le but de ce tuto est de vous aider à installer et configurer une Linux Mint afin de pouvoir l'utiliser pour du multimédia / Gaming.

En construction... Sujets à aborder :

## 1. Comment procéder à l'installation

Si besoin d'aide pour réaliser une clé bootable depuis Windows, vous pouvez consulter [cette page](https://emmabuntus.org/installer-emmabuntus-de5/#Avec_loutil_Etcher).

A compléter

## 2. Installation des pilotes Nvidia

A compléter

## 3. Mettre à jour son système et choisir ses mirroirs

A compléter

## 4. Modifier le vm.max_map_count (à faire jusqu'à la version 22 de Linux Mint)

Pour cela, il faut ouvrir un Terminal et taper : `sudo nano /etc/sysctl.conf`
Dans ce fichier, il faut uniquement ajouter la ligne suivante : `vm.max_map_count=2147483642`
Une fois fait, quitter le fichier en faisant `CTRL+X` et répondre oui pour sauvegarder.
Maintenant, il suffit de rédemarrer le PC et le tour est joué !

A noter qu'il est possible de vérifier que la valeur a bien été prise en compte en tapant dans un terminal la commande suivante : `sysctl vm.max_map_count`
Ce qui devrait renvoyer cette réponse : `vm.max_map_count = 2147483642`

Cette étape ne sera plus nécessaire avec la version 22.

## 5. Installer les logiciels

Une logithèque est mise à disposition sur Linux Mint pour installer vos applications. Pour accéder à celle-ci, il vous faut aller dans dans le menu des applications (1) et cliquer sur cette icône (2) :

![LM-acces-logitheque](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/ad2a9e25-274a-48fb-983d-f4e8d470ea7c)

Une fois ouverte, cela ressemblera à ceci :

![LM-logitheque-accueil](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/84b0a680-438e-455d-9951-7647504b6b55)

A partir de là, vous pouvez parcourir la liste des applications proposées ou faire une recherche ciblée. Par exemple, pour la partie gaming, vous aurez besoin d'installer Steam, il suffit donc de rechercher celui-ci :

![LM-logitheque-steam](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/35f8db07-d685-44cd-b927-f59f5cf0816b)

Ici, on peut voir plusieurs résultats et c'est les deux premiers qui vont nous intéresser. Le premier est un paquet système, c'est à dire un paquet dans les dépôts de la distribution et donc valider par celle-ci. Le second avec la mention "flatpak" est un paquet universel venant de flathub.

Les deux paquets vont fonctionner mais il est bon à noter de façons générales les points suivants :
- Les paquets systèmes sont souvent plus vieux (mais certains comme steam ont un système de mise à jour indépendant) et fonctionnent avec ce qui est installé sur le système ou fait ajouter des composants à votre système pour tourner.
- Les paquets flatpak tournent avec leur propre environnement et embarque tout avec eux (ce qui fait que leur taille est plus importante) et sont fournis dans la dernière version stable publiée et fonctionnent de la même manière avec tous les distributions. Ils ont aussi l'avantage de faire venir la dernière version de Mesa, ce qui est intéressant quand on utilise de l'Intel / AMD. En revanche, ils ont un accès limité au système, ce qui sécurise d'un côté mais rend certaines actions plus compliquées, notamment l'accès aux disques secondaires (voir [page suivante](https://github.com/Gaming-Linux-FR/glf-astuces?tab=readme-ov-file#acc%C3%A8s-%C3%A0-un-second-disque-sur-steam-flatpak)).

## 6. Désactivation de la composition des fenêtres

Désactiver la composition des fenêtres en plein écran (type jeu) permet d'avoir de meilleures performances.
Pour cela, il faut ouvrir le menu des applications (1) et ouvrir les paramètres système (2) :

![LM-desactivation-compo1](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/a4790345-ced0-459f-894b-7b4e79f649cf)

Puis aller dans `Général` :

![LM-desactivation-compo2](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/6abede6b-faba-48b8-a1e6-0409f5e3aa48)

Puis cocher l'option ci-dessous :

![LM-desactivation-compo3](https://github.com/Gaming-Linux-FR/guide-mint/assets/21110485/d89d66ce-6ebb-4970-b6f9-b3f6aa58bc78)
