---
layout: default
nav_order: 10 
title: Modèle 3D du couvercle
---

<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>

# Modèle 3D du couvercle

Nous avons modélisé le couvercle, si vous souhaitez le réaliser vous pouvez voir un aperçu ci-dessous. 
Le fichier est disponible dans les ressources du site.

<model-viewer
    id="viewer"
    alt="Modèle 3D du couvercle"
    src="../shared-assets/models/couvercle.gltf"
    poster="../shared-assets/images/couvercle.png"
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
