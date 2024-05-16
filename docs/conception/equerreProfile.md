---
layout: default
nav_order: 6
title: Equerre Profilés
parent: Conception et prototypage
---

<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>


<model-viewer 
    id="viewer" 
    alt="Modèle 3D du bras robot Niryo Ned 2" 
    src="../shared-assets/models/equerreFixe.gltf" 
    poster="../shared-assets/images/equerreFixe.png" 
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