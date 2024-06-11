---
layout: default
nav_order: 3
title: mallette 3
parent: Conception et prototypage
---

# Mallette 3

## Croquis

<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>

![Plan de la mallette](../shared-assets/images/dessin_mallette3_vue_dessus.png)
![Plan de la mallette](../shared-assets/images/dessin_mallette3_vue_cote.png)
![Plan de la mallette](../shared-assets/images/dessin_mallette3_couvercle.png)

---

## Modèle 3D

<model-viewer
    id="viewer"
    alt="Modèle 3D du bras robot Niryo Ned 2"
    src="../shared-assets/models/3D_REPRESENTATION.gltf"
    poster="../shared-assets/images/3D_REPRESENTATION.png"
    shadow-intensity="1"
    camera-controls
    touch-action="pan-z"
    rotation="0 0 90">
</model-viewer>

---

## Prototypage

Nous avons réalisé un prototype à l'échelle 1/10 des dimensions souhaitées pour le prototype final.
Ce prototype nous permettra d'éviter des erreurs futures lors de la conception. En effet, on a constaté qu'il manquait les coins sur les longueurs de la boîte.
On ajustera donc les dimensions du prototype final pour pouvoir obtenir un rectangle régulier.
Seul un côté restera sans coin, celui de la liaison des deux parties du socle puisque celles-ci doivent pouvoir s'aligner côte à côte.

![Photo socle](../shared-assets/images/proto_socle.jpg)
Photo du socle déplié, le scotch représente la charnière permettant la rotation des deux parties.

![Photo socle et couvercle](../shared-assets/images/proto_separe.jpg)
Photo du socle et du couvercle séparé.

![Photo boite](../shared-assets/images/proto_boite.jpg)
Photo de la boîte fermée lorsque le couvercle est posé sur le socle. Sur ce prototype, rien ne permet d'attacher le socle et le couvercle ensemble mais sur le prototype final ce sera fait grâce à des [sauterelles](../conception/supportCharniere.md).

![Photo couvercle ouvert](../shared-assets/images/proto_couvercle_ouvert.jpg)
Photo de la boîte avec le couvercle du coffre ouvert, ici aussi le scotch fais office de charnière.

<style>
    #viewer
    {
        margin : auto;
        width : 500px;
        height : 500px;
    }
</style>