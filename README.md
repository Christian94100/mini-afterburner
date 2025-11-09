# mini-afterburner
mini-afterburner en code C 


# Mini Afterburner en C avec SDL2

Jeu simple en C inspiré d'Afterburner (1991) utilisant SDL2.

## Compilation et lancement

# Mini Afterburner en C avec SDL2

Ce projet est un jeu simple inspiré d'Afterburner (1991), développé en C avec la bibliothèque SDL2. Il sert de base pour apprendre la programmation de jeux 2D.

## Fonctionnalités

- Fenêtre graphique avec SDL2
- Mouvement fluide de l’avion contrôlé par les flèches du clavier
- Tir de projectiles avec la barre espace
- Scrolling horizontal basique du fond
- Limites de déplacement pour le joueur

## Prérequis

- SDL2 doit être installée sur ton système.

### Installation de SDL2

- Sur Debian/Ubuntu :  
sudo apt install libsdl2-dev

text
- Sur Windows : télécharge et installe SDL2 depuis le site officiel https://www.libsdl.org/download-2.0.php

## Compilation

Compile le projet avec gcc en liant SDL2 :

gcc afterburner.c -o afterburner -lSDL2

text

## Lancement

Execute le programme :

./afterburner

text

## Améliorations possibles

- Ajouter des ennemis avec mouvements et destructions  
- Gestion des collisions et vie du joueur  
- Ajout de sons et musiques  
- Intégration de vraies images (sprites) pour le décor et le joueur  
- Score et interface utilisateur  
- Mise en place de niveaux et challenges

## Licence

