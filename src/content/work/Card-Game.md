---
title: Jeu de cartes
publishDate: 2023-02-01 00:00:00
img: /assets/Cardgame/Cartes.png
img_alt: Cartes
description: |
  Programmation d'un jeu de cartes dans un terminal
tags:
  - Programmation
  - C++
  - Terminal
  - Jeu de cartes
  - Travail en binôme
---

##### Décembre 2022 - Février 2023

Développement d'un jeu de cartes type "Yu-Gi-Oh" (C++) en binôme, dans un terminal.

## Annexes

#### Règles

L'utilisateur lance le programme puis choisis entre le mode PVE (Player vs Environment) ou PVP (Player vs Player).
Il entre ensuite son pseudo et les règles lui sont affichées.

> ![Règles](/assets/Cardgame/Règles.png "Titre facultatif")

#### Affichage des cartes

La liste des cartes disponibles lui est affichée, il devra ensuite choisir son deck (son jeu de carte).

> ![Cartes](/assets/Cardgame/Cartes.png "Titre facultatif")

#### Choix du deck

Le joueur doit désormais choisir la manière dont son deck sera trié :

- "dumb" (tri automatique par dégats d'attaque, défense ou dégâts magiques)
- "smart" (tri automatique laissant le choix au joueur de l'importance de chaque attribut)
- "score" (tri automatique combinant les dégâts d'attaque, la défense et les dégâts magiques)

Suite à ça, le joueur a le choix de trier son deck de manière croissante ou décroissante.

> ![Génération_cartes](/assets/Cardgame/Génération_cartes.png "Titre facultatif")

#### Début de la partie

Une fois le jeu lancé, les cartes des decks des deux joueurs s'affrontent

> ![Début_partie](/assets/Cardgame/Début_partie.png "Titre facultatif")

#### Fin de la partie

Une fois qu'un des deux joueurs a un nombre de prestige inférieur ou égale à zéro, la partie est terminée et l'autre joueur remporte la partie.

Le joueur a ensuite la possibilité de recommencer une partie ou de quitter le jeu.

> ![Fin_partie](/assets/Cardgame/Fin_partie.png "Titre facultatif")
