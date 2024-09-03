---
layout: default
nav_order: 7
title: Armature de la boîte
parent: Études et choix techniques
---
<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>

# Pourquoi une armature ?

Nous avons comme contrainte d'utiliser la découpeuse laser de l'école afin de réaliser notre mallette en planche de peuplier de 5mm. Cependant, avec la masse importante de matériel se trouvant dans la mallette, il est certain que des planches de 5mm ne suffieraient pas.
Nous avons étudié la possibilité de doubler l'épaisseur en réalisant la mallette avec deux couches de 5mm. La mallette était assez grande, cette possibilité nécessitait un nombre de planches conséquant. Pas le choix, nous avions besoin de trouver une alternative.
De cette conclusion résulte l'armature. En effet, une armature réalisé à partir de profilés de 20x20mm recouverte d'une planche de peuplier de 5mm semblait être la meilleure solution respectant nos contraintes.

<model-viewer
    id="viewer"
    alt="Modèle 3D de l'armature"
    src="../shared-assets/models/armature.gltf"
    poster="../shared-assets/images/capture_armature.png"
    shadow-intensity="1"
    camera-controls
    touch-action="pan-z"
    rotation="90 90 90">
</model-viewer>

<style>
    #viewer
    {
        margin : auto;
        width : 500px;
        height : 500px;
    }
</style>

Nous pouvons donc réaliser cette armature pour la base de la mallette ainsi que pour le côté accueillant le plateau des grilles modulaires. voir [mallette 3](../conception/mallette_3.html).
