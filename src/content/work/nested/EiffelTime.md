---
title: Application de gestion universitaire (web/iOS/android)
publishDate: 2025-01-27 20:00:00
img: /assets/EiffelTime/Login_screen.png
img_alt: Page de connexion
description: |
  Conception et développement d'une application de gestion universitaire multiplateforme
tags:
  - React
  - React Native
  - Tailwind
  - TypeScript
  - Vite.js
  - Design UI/UX
  - Front-End
---

## Introduction

Eiffel Time est une application de gestion universitaire, ayant pour objectif de centraliser et de faciliter la gestion des notes, le suivi des présences des élèves et des enseignants, la communication et l’emploi du temps.

## Contexte et Objectifs

Dans le cadre d'un projet interne à l'IUT de Marne-la-Vallée, nous avons conçu et développé une application de gestion universitaire multiplateforme, sur web, iOS et android,
ayant pour objectif de centraliser et de faciliter la gestion des notes, le suivi des présences des élèves et des enseignants, la communication et l’emploi du temps.
Ce projet répond à un besoin au sein de l'IUT, jusqu'à lors, les présences des élèves et des enseignants, étaient suivies à travers des feuilles d'émargement,
que les secrétaires de chaque département récupèrent après chaque cours, avant des remplir des tableaux excel contenant les absences pour chaque étudiants,
et les présences pour chaque enseignants. De plus les notes des évaluations étaient manuscrites, et transmises aux secrétariats sous forme de tableau avec les notes
pour chaque élève d'une classe. Ce système, posait de gros problèmes de temps et d'accessibilité, car tout était fait manuellement, ce qui fait que les élèves
devaient se rendre au secrétariat pour accéder à leurs absences et leurs notes. De plus, les enseignants devaient se rendre au secrétariat pour récupérer la feuille d'émargement
avant chaque cours, puis la remettre après chaque cours.

## Tâches

Ce projet étant décomposé en plusieurs phases tout au long de l'année, je vais présenter sur cette page chacune de mes contributions.

### Recueil des besoins

Pour la partie recueil des besoins, j'ai rédigé un questionnaire regroupant une quinzaine de questions pour mieux cerner les besoins de chacun des acteurs principaux
concerné par ce projet : l'équipe administrative du CRI (centre de ressources informatiques), le chef du département informatique, la secrétaire, les enseignants et les élèves.
Suite à cela, je me suis entretenu avec la secrétaire et le chef du département informatique pour comprendre quelles sont les fonctionnalités auxquelles ils aimeraient accéder sur la future application.

### Spécifications

Le recueil des besoins m'a permis de mieux comprendre les fonctionnalités attendues, et donc de concevoir un diagramme PBS (Product Breakdown Structure),
pour décomposer le produit final en sous-produits, jusqu'à atteindre un niveau de détail suffisamment clair pour l'équipe.
Ce diagramme PBS m'a servi de base pour concevoir un diagramme WBS (Work Breakdown Structure), qui s'est avéré très utile notamment pour la planification et l'organisation du projet
au sein de l'équipe.

#### Product Breakdown Structure

> ![PBS](/assets/EiffelTime/PBS.jpg "PBS")

#### Work Breakdown Structure

> ![WBS](/assets/EiffelTime/WBS.jpg "WBS")

### Conception et prototypage

Durant la conception et le prototypage, je me suis chargé dans un premier temps de concevoir les maquettes sur figma, pour la partie web, puis j'ai ensuite prototypé ces maquettes pour avoir une "fake app" permettant d'avoir une idée de l'interface utilisateur,
et commencer à réfléchir à certaines problématiques liées à l'expérience utilisateur.

Suite à cela, je suis allé m'entretenir avec les acteurs principaux, tels que le chef et la secrétaire du département informatique afin d'obtenir leurs retours sur les maquettes, et de m'assurer que je n'avais rien oublié concernant leurs besoins.

#### Maquette web

<iframe 
  style="border: 1px solid rgba(0, 0, 0, 0.1);" 
  width="800" 
  height="450" 
  src="https://embed.figma.com/proto/ziuFNyjNjHjuCIvytgZ6R6/Maquette?page-id=0%3A1&node-id=59-52&viewport=2883%2C-1130%2C0.16&scaling=scale-down&content-scaling=fixed&starting-point-node-id=59%3A52&show-proto-sidebar=1&embed-host=share&theme=dark" 
  allowfullscreen>
</iframe>

#### Maquette mobile

Pour la partie mobile, j'ai essayé de reproduire le plus d'écrans possibles similairement à la version web, car j'avais déjà à ce
moment pour idée de développer l'application web et l'application mobile avec un maximum de composants partagés.
Les maquettes de la version mobile sont donc très similaires à la version web, sauf quelques points qui ont été ajusté pour des
raisons d'expérience utilisateur, notamment comme la barre de navigation latérale de la version web (sidebar) qui a été remplacé par une barre d'onglet en bas de l'écran sur mobile.

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);"
 width="800" 
 height="450" 
 src="https://embed.figma.com/proto/ziuFNyjNjHjuCIvytgZ6R6/Maquette?page-id=569%3A977&node-id=835-1745&p=f&viewport=25%2C359%2C0.04&scaling=scale-down&content-scaling=fixed&starting-point-node-id=835%3A1745&show-proto-sidebar=1&embed-host=share&theme=dark"
 allowfullscreen>
</iframe>
