---
layout: default
nav_order: 10
title: Modélisation
parent: Études et choix techniques
---
<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>

Cette page sert à regrouper les différentes études concernant les modélisations 3D que nous avons réalisé.

## Butée

Afin de fermer la boîte, nous avons besoin d'un système qui permet de tenir celle-ci en angle droit afin de faciliter sa fermeture avec le couvercle. Nous avons donc modélisé un sytème de butée fixée à la boîte.
[butée](../conception/butee.html)

## Pièce de support pour la charnière

Pour pallier le problème de solidité au niveau de la charnière (voir [Charnière](charniere.html)) nous avons choisi de créer une pièce en modélisation 3D qui se fixera sur les profilés ainsi que sur la charnière.
Le but de cette pièce est de soulager la charnière. En effet, nous craignons que celle-ci, uniquement fixée dans une planche de 5mm, ne puisse pas supporter la masse qui lui sera appliquée. Nous avons donc conçu cette [pièce](../conception/supportCharniere.html).

## Equerre pour Profilés

Afin de fixer nos profilés ensemble, nous avons pensé à utiliser ce système :

<model-viewer
    id="viewer"
    alt="Modèle 3D du bras robot Niryo Ned 2"
    src="../shared-assets/models/equerreProfiles.gltf"
    poster="../shared-assets/images/equerreProfiles.png"
    shadow-intensity="1"
    camera-controls
    touch-action="pan-z"
    rotation="90 90 90">
</model-viewer>

Le problème est que nous ne pouvons pas fixer ce genre d'équerre avec le budget restant, par conséquence, nos profilés sont libres et n'ont pas une position fixe.
Nous avons donc décidé de concevoir notre propre équerre : [equerre pour profilés](../conception/equerreProfile.html), nous pourrons la fixer en utilisant du matériel mis à notre disposition.

<style>
    #viewer
    {
        margin : auto;
        width : 500px;
        height : 500px;
    }
</style>
