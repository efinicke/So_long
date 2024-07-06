# SO LONG
[MiniLibX Documentation](https://harm-smits.github.io/42docs/libs/minilibx/introduction.html)


## 1. Skills

- **Window management and graphical display with a graphical library "MiniLibX"**
- **event handling (keyboard and mouse)**
- **Use of textures and sprites**
- **Programming in C according to the Norm**
- **Files manipulation**
- **map parsing**
- **Dynamic memory management**
- **Structures management**
- **Makefile creation**
- **Clean code**


## 2. Project Overview

"So long" est un de mes projet 42 qui m'a appris à coder un jeu 2D simple et fonctionnel en C où le joueur contrôle un personnage qui doit collecter des items et atteindre la sortie sur une carte définie, et donc à intégrer l'usage d'une librairie graphique dans mon code. Le jeu utilise en effet la bibliothèque graphique MiniLibX pour l'affichage et la gestion des événements. Il m'a permis de créer et utiliser des sprites pour l'affichage et à gérer les interractions utilisateur via le clavier.


## 3. Features

Le programme inclut les fonctionnalités suivantes :
- Déplacement du personnage avec les touches W, A, S, D
- Affichage des mouvements du personnage dans le shell
- Collecte d'items sur la carte
- Vérification des collisions avec les murs
- Affichage en 2D de la carte, des items, et des murs
- Fermeture propre de la fenêtre avec la touche ESC ou en cliquant sur la croix


## 4. Content

Le projet contient les fichiers suivants :
- **Fichiers srcs, includes, de compilation**: *.c, *.h, Makefile
- **maps**: *.ber
- **Sprites et textures**: images de jeu
- **Bibliothèque MiniLibX**: fichiers de la bibliothèque
- Mlx


## 5. Usage

1. ### Installation 
La Mlx est déjà téléchargée et intégrée dans le projet, mais il faut aussi installer X11 et Xext sur votre système. La minilibx de 42 utilise ces bibliothèques pour l'affichage graphique : 
```bash
    sudo apt-get update
    sudo apt-get install libx11-dev libxext-dev
```

Il faudra aussi installer la bibliothèque libbsd : 
```bash
    sudo apt-get update
    sudo apt-get install libbsd-dev
```

2. ### Compilation 
Compiler le projet avec le Makefile fourni dans le dossier `project` :
```sh
   make
```

3. ### Execution

Utiliser le fichier .ber de son choix en remplacant l'étoile par le nom du fichier (les maps incluent les fichiers de test d'erreur de parsing)

```bash
    ./so_long maps/*.ber
```


## Links 

"MiniLibX is a tiny graphics library which allows you to do the most basic things for rendering something in screens without any knowledge of X-Window and Cocoa. It provides so-called simple window creation, a questionable drawing tool, half-ass image functions and a weird event management system."

To understand how to use the Mlx in your code : 
[MiniLibX Documentation](https://harm-smits.github.io/42docs/libs/minilibx/introduction.html)