---
layout: default
title: Module tri avec kit vision
parent: Programmation
nav_order: 1
---

# Module de tri avec kit vision

Comme expliqué précédemment, notre premier module est un module de tri. Ce tri sera fait par les couleurs et/ou par les formes.

## L'objectif

Dans ce module nous cherchons à reproduire une chaîne de tri basique. Nous cherchons donc à trier les objets venant du convoyeur.

## Sa réalisation

Tout d'abord, ce module utilise le kit vision. Il faut donc le paramétrer. Pour ce faire nous avons à disposition 4 cibles à fixer sur les côté du convoyeur. 
Une fois les cibles installer, il est nécessaire d'enregistrer leurs positions dans le robot afin qu'il puisse les utiliser. C'est à ce moment que nous devons utiliser la pointe de précision. 
Nous venons positionner la pointe au centre de la cible grâce au bouton "freemotion" sur le côté du bras. Une fois positionner, on appui sur le bouton "save" présent à la gauche du bouton précédent. On répète donc ces étapes pour les 3 autres cibles. 
Cette initialisation de la zone de travail est à faire à chaque fois que nous la déplacons à une nouvelle place mais plusieurs zone peuvent être paramétrer dans le robot. 


Ensuite nous allons pouvoir nous concentrer sur le module en lui même. 

Ce module se divise en plusieurs programmes. 

Dans un premier temps, nous avons choisi de mettre en place le tri par couleur. Pour ce faire, nous placons le robot afin que le kit vision puisse voir l'intégralité de la zone de travail choisi. Une fois bien positionné nous choisissons de scanner en continu la zone. Une fois qu'un objet y rentre, nous stoppons le convoyeur. Par la suite, le robot analyse l'objet (uniquement la couleur dans ce cas). Une fois l'analyse effectué, le robot réagi en conséquence en saisissant l'objet puis en le déplacant à l'endroit prédéfini pour la couleur. Une fois l'objet déplacer, le convoyeur se remet en marche et le robot reviens se mettre à sa position d'observation. Le programme se réexécute continuellement tant que la sécurité n'est pas atteinte. La sécurité est donc un compteur qui s'incrémente à chaque fois que le programme regarde dans la zone de travail et qu'il n'y a rien. Une fois arrivé à 50 le robot reviens se mettre dans une position d'attente, le convoyeur s'arrête et le programme se termine. La valeur de la sécurité repasse à 0 à chaque fois que la caméra détecte un objet dans la zone de travail.

Une fois ce programme fonctionnel, nous décidons de s'attaquer au code permettant le tri par forme. Nous utilisons le même algorithme à l'execption que le robot fait le choix en fonction de la couleur et non de la forme.

Les deux précédents tris ne nous permette pas de choisir un objet ou une couleur que nous souhaitons. Cela fais l'objet du troisième programme. Dans ce cas, nous demandons à l'utilisateur de choisir la couleur de leur choix (rouge par défaut) et sa forme (carré par défaut) afin de pouvoir sélectionner uniquement les objets de la couleur et de la forme choisi.
Dans ce cas, nous avons deux positions de stockage des éléments triés. Le premier est celui où nous avons les objets souhaités et le second comporte les objets necorrespondant pas au(x) critère(s).

Par la suite, nous nous devons de réaliser des ressources pédagiques afin de permettre au élève de prendre en main facilement et rapidement le robot tout en assurant la sécurité de chaque personne pouvant entrer en contact avec le robot. Pour ce faire, nous proposons 2 types de codes pédagogiques. 
La première proposition est un code à remmettre dans l'ordre où il y a tout les blocks de codes écrit mais divisé en plusieurs petits codes. L'objectifs de cette ressource est de permettre aux élèves d'utiliser le robot sans se préocupper de l'utilisation des systèmes de mouvements. 
La seconde proposition est un code à remplir selon les envies de l'utilisateur. Pour ce faire, nous allons fournir architecture globale du code et laisser vide les valeurs de déplacements. Cela permettra aux élèves de se familiariser avec les déplacements du robot et de leur effets. 


**Une fois ces deux types d'exercices réaliser les élèves seront capable de faire leur propre programme basique avec le robot, son convoyeur et son kit vision.**