---
layout: default
title: Module tri avec kit vision
parent: Programmation
nav_order: 1
---

# Module de tri avec kit vision

Comme expliqué précédemment, le premier module est un module de tri. Ce tri sera fait par les couleurs et/ou par les formes.

## L'objectif

Ce module reproduit une chaîne de tri basique. Il trie donc les objets venant du convoyeur.

## Sa réalisation

Tout d'abord, ce module utilise le kit vision. Il faut donc le paramétrer. Pour ce faire, il est mis à disposition 4 cibles à fixer sur les côtés du convoyeur. 
Une fois les cibles installer, il est nécessaire d'enregistrer leurs positions dans la mémoire du bras robot afin qu'il puisse les utiliser. C'est à ce moment qu'il faut utiliser la pointe de précision fourni dans le kit vision. 
Pour enregistrer chaque cible, il faut positionner la pointe au centre de cette dernière grâce au bouton "freemotion" sur le côté du bras. Une fois positionné, on appui sur le bouton "save" présent à côté du bouton précédent. On répète donc ces étapes pour les 3 autres cibles. 
Cette initialisation de la zone de travail est à faire à chaque fois qu'elle est déplacé à une nouvelle place mais plusieurs zones peuvent être paramétré dans le cobot. 


Maintenant que cela est fait, il faut se concentrer sur le module en lui même.

Ce module se divise en plusieurs programmes. 

Dans un premier temps,  choisi de mettre en place le tri par couleur. Pour ce faire, il faut articuler le bras robotisé afin que le kit vision puisse voir l'intégralité de la zone de travail choisi. Une fois bien positionné, la caméra scanne la zone en continu. Une fois qu'un objet y rentre, le cobot envoi la consigne de stopper le convoyeur. Par la suite, la caméra analyse l'objet (uniquement la couleur dans ce cas). Une fois l'analyse effectué, le cobot réagi en conséquence en saisissant l'objet puis en le déplacant à l'endroit prédéfini pour la couleur. Une fois l'objet déplacer, le convoyeur se remet en marche et le cobot se remet à sa position d'observation. Le programme se réexécute continuellement tant que la sécurité n'est pas atteinte. La sécurité est donc un compteur qui s'incrémente à chaque fois que le programme regarde dans la zone de travail et qu'il n'y a rien. Une fois arrivé à 50 (ce qui correspond à 15 secondes environ), le cobot reviens se mettre dans une position d'attente, le convoyeur s'arrête et le programme se termine. La valeur de la sécurité repasse à 0 à chaque fois que la caméra détecte un objet dans la zone de travail.

Une fois ce programme fonctionnel, il faut s'attaquer au code permettant le tri par forme. Pour ce faire, le même algorithme sera utiliser à l'exception que le cobot fait le choix en fonction de la forme et non de la couleur.

Les deux précédents tris ne permette pas de choisir un objet ou une couleur que l'utilisateur. Cela fais l'objet du troisième programme. Dans ce cas, il est demandé à l'utilisateur de choisir la couleur de leur choix (rouge par défaut) et sa forme (carré par défaut) afin de pouvoir sélectionner uniquement les objets de la couleur et de la forme choisi.
Dans ce cas, il existent deux positions de stockage des éléments triés. Le premier est celui où les objets souhaités seront déposés et le second comporte les objets ne correspondant pas au(x) critère(s).

Par la suite, il faut s'attaquer à la réalisation des ressources pédagogiques afin de permettre au élève de prendre en main facilement et rapidement le cobot Niryo Ned 2 tout en assurant la sécurité de chaque personne pouvant entrer en contact avec le robot collaboratif. Pour ce faire, il existe 2 types de codes pédagogiques. 
La première proposition est un code à remmettre dans l'ordre où il y a tout les blocks de codes écrit mais divisé en plusieurs petits codes. L'objectif de cette ressource est de permettre aux élèves d'utiliser le cobot sans se préocupper de l'utilisation des systèmes de mouvements. 
La seconde proposition est un code à remplir selon les envies de l'utilisateur. Pour ce faire, il sera fourni une architecture globale du code et les valeurs de déplacements seront laisser vides. Cela permettra aux élèves de se familiariser avec les déplacements du cobot et de leur effets. 

Il est important de noter que des étapes positions intermédiaire ont été paramétré afin que le cobot ne rentre pas en collision avec d'autres objets pendant l'éxecution du programme.

**Une fois ces deux types d'exercices réaliser les élèves seront capable de faire leurs propres programmes basiques avec le cobot Niryo Ned 2, son convoyeur et son kit vision.**