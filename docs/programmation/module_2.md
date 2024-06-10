---
layout: default
title: Module transfert
parent: Programmation
nav_order: 2
---

# Module de tri avec kit vision

Comme expliqué précédemment, le second module est un module de transfert sur le convoyeur

## L'objectif

Ce module viens donc chercher un objet à une position défini puis le deplace sur le début du convoyeur.

## Sa réalisation

Ce module se décompose en deux parties. 

Le premier est la prise de l'objet. Pour la faire, il faut enregister la zone de récupération des objets. Il faut donc positionner le cobot à la position voulu grâce au bouton "freemotion" sur le côté du bras. Une fois positionné, on appui sur le bouton "save" pour récupérer la position dans notre programme.

Pour la seconde étape, il faut enregistrer la position à laquelle le cobot va déposer l'objet. On répète l'étape précedente mais en positionnant le bras robot à la nouvelle position voulu. 

Une fois les deux position connu, il suffit de mettre une boucle qui fera les va-et-vient entre la position de ramassage de l'objet et la position de dépôt. 
Il faut tout de même faire attention que la trajectoire du cobot ne vienne pas renconter d'autres objets placés.

Par la suite, il faut s'attaquer à la réalisation des ressources pédagogiques afin de permettre au élève de prendre en main facilement et rapidement le robot tout en assurant la sécurité de chaque personne pouvant entrer en contact avec le robot. Pour ce faire, il existe 2 types de codes pédagogiques. 
La première proposition est un code à remmettre dans l'ordre où il y a tout les blocks de codes écrit mais divisé en plusieurs petits codes. L'objectif de cette ressource est de permettre aux élèves d'utiliser le robot sans se préocupper de l'utilisation des systèmes de mouvements. 
La seconde proposition est un code à remplir selon les envies de l'utilisateur. Pour ce faire, il sera fourni une architecture globale du code et les valeurs de déplacements seront laisser vides. Cela permettra aux élèves de se familiariser avec les déplacements du robot et de leur effets. 

Il est important de noter que des étapes positions intermédiaire ont été paramétré afin que le cobot ne rentre pas en collision avec d'autres objets pendant l'éxecution du programme.

**Une fois ces deux types d'exercices réaliser les élèves seront capable de faire leurs propres programmes basiques avec le cobot et son convoyeur.**