---
title: Application mobile de stimulation cognitive
publishDate: 2024-07-10 00:00:00
img: /assets/Test.png
img_alt: Pearls of silky soft white cotton, bubble up under vibrant lighting
description: |
  Refonte et migration d'une application de stimulation cognitive
tags:
  - Développement d'application mobile
  - Android
  - Java
  - Autonomie
---

## Introduction

L'objectif de ce projet était de permettre le lancement d'une application A, directement depuis une autre application B, et de réaliser la refonte de l'application A, pour qu'elle suive la même charte graphique que l'application B.

## Contexte

L'application A se nomme en réalité SelfCog, une application de stimulation cognitive, utilisée dans des établissements de santé telles que des cliniques.
SelfCog permet à un professionnel de se connecter avec ses identifiants, de créer une étude clinique, puis de faire réaliser au patient cinq tests composés chacun de quarante exercices :

- Test moteur
- Test visuel
- Test du langage
- Test des fonctions exécutives
- Test de mémoire

Chaque fois que le patient termine un test, plusieurs calculs sont réalisés en fond par l'application, puis des résultats tels que le score obtenu au test, le temps de réaction et l'IES (Index d'Efficacité de Signal) sont stockés dans un fichier CSV puis dans un fichier HTML. Ces deux fichiers comportent les résultats de l'étude clinique et le professionnel peut y avoir accès en s'y connectant avec les identifiants de l'étude clinique.

Jusqu'à lors, cette application datant de 2014 était utilisée uniquement de manière indépendante. Depuis l'entreprise Dynseo a créé d'autres applications permettant de réaliser des études cliniques, telles que Calap, Selfdiag, ou encore Voice.

Certains clients ont alors manifesté leur intérêt pour une seule application, réunissant toutes ces autres applications : CogTel (que j'ai appelé application B dans l'introduction).

## Objectifs

Un des objectifs de ce projet étant donc de permettre au professionnel de lancer SelfCog depuis Cogtel, sans avoir à recréer un compte sur SelfCog, ni de devoir se reconnecter sur SelfCog, ni même de créer une étude clinique sur SelfCog.

Tout doit être fait depuis CogTel. Pour cela, les deux applications doivent communiquer entre elles : CogTel doit transmettre différentes informations à SelfCog sous forme de JSON, telles que les données du patient ainsi qu'une étude clinique déjà pré-réalisée sur CogTel. SelfCog doit ensuite pouvoir extraire ces informations du JSON et les intérpréter pour initialiser une session ainsi qu'une étude clinique.

En lançant SelfCog depuis CogTel, le professionnel doit donc directement arriver sur la première page du tutoriel sans avoir à re-remplir un formulaire d'étude clinique, ni même ses identifiants.

CogTel transmet donc toutes les informations nécessaires à SelfCog sous forme de JSON, dans un intent et attend un résultat de la part de SelfCog, ce qui fait que lorsque le patient appuie sur le bouton pour revenir à l'accueil, les résultats des tests de l'étude clinique doivent aussi être transmis sous forme de JSON, dans un intent.

Toutes ces étapes doivent désormais être exécutées en fond.

J'ai donc collaboré avec la personne qui travaillait sur CogTel afin que nos deux applications puissent communiquer entre elles.

Le deuxième objectif de ce projet, comme je l'ai dis plutôt dans l'introduction, était de réaliser la refonte graphique de SelfCog, qui était vieille de dix ans, pour qu'elle suive la même charte graphique de CogTel.

Pour cela j'ai reproduis dans le code les maquettes que ma cheffe de projet avait réalisé, en suivant les instructions qu'elle m'a donné.

## Annexes

### Avant

##### Ci-dessous, vous trouverez les écrans qui sont nécessaires dans le cas d'une connexion sur SelfCog de façon indépendante mais à enlever dans le cadre d'une connexion depuis CogTel

#### Ancien écran login

> ![Ecran login selfcog](/assets/LoginSelfcog.png "Ecran login")

#### Ancien écran formulaire

> ![Ecran formulaire selfcog](/assets/FormulaireSelfcog.png "Ecran formulaire")

#### Ancien écran login admin

> ![Ecran login admin selfcog](/assets/LoginAdmin.png "Ecran login admin")

#### Ancien écran pour ajouter une étude clinique

> ![Ecran ajout étude selfcog](/assets/AjoutEtude.png "Ecran ajout étude")

#### Anciens écrans de résultat d'étude clinique

> ![Ecran résultat étude selfcog](/assets/ResultatsEtude1.png "Ecran résultat étude") ![Ecran résultat étude 2 selfcog](/assets/ResultatsEtude2.png "Ecran résultat étude 2") ![Ecran résultat étude 3 selfcog](/assets/ResultatsEtude3.png "Ecran résultat étude 3")

#### Ancien écran de gestion d'étude

> ![Ecran gestion étude selfcog](/assets/GestionEtudes.png "Ecran gestion étude")

### Lancement de SelfCog depuis CogTel

> ![Ecran cogtel selfcog](/assets/EcranCogtel.png "Ecran cogtel selfcog")

### Après

#### Nouveaux écrans de tutoriel

> ![Ecran tuto1 selfcog](/assets/Tuto1.png "Ecran tuto1") ![Ecran tuto2 selfcog](/assets/Tuto2.png "Ecran tuto2") ![Ecran tuto3 selfcog](/assets/Tuto3.png "Ecran tuto3")

#### Exemple de nouveaux écrans d'instruction

> ![Ecran instruction1 selfcog](/assets/Instruction1.png "Ecran instruction1") ![Ecran instruction2 selfcog](/assets/Instruction2.png "Ecran instruction2")

#### Exemple de nouvel écran d'exercice pendant un test

> ![Ecran Test selfcog](/assets/Test.png "Ecran test")
