---
layout: default
nav_order: 2
title: Module Chaine de tri
parent: Modules
---

# Chaîne de Tri

Cette application est la première idée que nous avons eu en commençant le projet.

## Fonctionnement

L'utilisateur doit d'abord placer le robot à l'emplacement lié à la démonstration comme ci-dessous.

![photos montrant le placement robot](../shared-assets/images/placement_robot.jpg)

Par la suite, il faut placer les 3 plaques qui recevront les objets triés.

## Matériel

Pour ce module, nous avons besoin :

- Un convoyeur qui va amener les objets au bras robot
- Le bras robot
- Des capteurs pour la couleur et la forme des objets
- Des plaques pour recevoir les objets triés

## Le kit Vision de Niryo

Niryo met en vente beaucoup d'accessoires pouvant compléter le bras robot, parmi ceux-ci, nous retrouvons le kit Vision.

![animation gif du kit vision de niryo](../shared-assets/video/visionGIF.gif)

<br>

Le kit Vision nous permet de faire de la reconnaissance de forme et de couleur, parfait pour notre module.
Nous utiliserons uniquement les trois couleurs des objets fournis (rouge, vert et bleu) ainsi que leurs deux formes utilisées (rond et carré).
Le kit vision comprend :

- Une zone de travail
- Une caméra
- Des objets à manipuler
- Une pointe de précision

La zone de travail est une zone créée par 4 "balises" permettant à la caméra de se repérer.

![image de la zone de travail du kit vision](../shared-assets/images/zoneTravailVision.png)

## Et après le tri ?

L'utilisateur renseigne donc la façon dont il veut trier ses objets et le bras fait tout le reste. Les objets lui sont amenés via un convoyeur et il les range ensuite dans leur boîte attitrée.
Par exemple, si l'utilisateur veut trier les objets par couleur et ne garder que la couleur <span style="color:green;">verte</span>, alors il aura besoin de deux contenant : un pour les objets verts, et un pour le reste.

*Source : https://niryo.com/fr/produits-cobots/ensemble-de-vision-ned2/*