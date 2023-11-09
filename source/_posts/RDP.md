---
title: Utiliser Deux Écrans avec le Protocole de Bureau à Distance (RDP)
date: 2023-11-08 23:54:51
tags: jalarue teletravail
---

## Introduction

Le Protocole de Bureau à Distance (RDP) de Microsoft permet aux utilisateurs de se connecter à un ordinateur distant et de l'utiliser comme s'ils étaient sur place. L'utilisation de deux écrans en RDP peut augmenter la productivité en offrant plus d'espace de travail.

<!-- more -->

## Étape 1 : Configuration des Écrans Locaux

Avant de démarrer une session RDP, assurez-vous que vos deux moniteurs sont correctement configurés sous Windows.

1. Faites un clic droit sur le bureau et sélectionnez `Paramètres d'affichage`.
2. Sous `Plusieurs écrans`, assurez-vous que l'option `Étendre ces affichages` est sélectionnée.

## Étape 2 : Lancement de la Connexion Bureau à Distance

Ouvrez le programme `Connexion Bureau à Distance` en tapant `mstsc` dans la barre de recherche Windows.

## Étape 3 : Configuration de la Session RDP pour Deux Écrans

Dans la fenêtre de la Connexion Bureau à Distance, suivez ces étapes pour activer l'utilisation de deux écrans :

1. Cliquez sur `Afficher les options`.
2. Dans l'onglet `Affichage`, cochez l'option `Utiliser tous mes écrans pour la session à distance`.
   ![RDP](/images/RDP.jpg)
3. Vous pouvez également ajuster la résolution de chaque écran si nécessaire.

## Étape 4 : Connexion

Entrez les informations de l'ordinateur distant et connectez-vous. Votre session RDP devrait maintenant s'étendre sur les deux écrans.

## Conseils Supplémentaires

- Si vous avez des problèmes avec l'affichage sur plusieurs moniteurs, vérifiez que le système d'exploitation de l'ordinateur distant prend en charge cette fonctionnalité.
- Vous pouvez également utiliser des paramètres de ligne de commande pour démarrer une session RDP avec plusieurs moniteurs en utilisant le flag `/multimon`.

## Conclusion

Utiliser deux écrans avec RDP peut rendre votre travail à distance beaucoup plus efficace. Assurez-vous de configurer correctement à la fois vos écrans locaux et les paramètres RDP pour profiter pleinement de cette fonctionnalité.
