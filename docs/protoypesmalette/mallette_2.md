---
layout: default
nav_order: 3
title: mallette 2
parent: Conception et prototypage
---
<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>

<model-viewer 
    id="viewer" 
    alt="Modèle 3D du bras robot Niryo Ned 2" 
    src="../shared-assets/models/mallette_2.gltf" 
    poster="../shared-assets/images/capture_niryo.jpg" 
    shadow-intensity="1" 
    camera-controls 
    touch-action="pan-z"
    rotation="0 0 90">
</model-viewer>

<style>
    #viewer
    {
        margin : auto;
        width : 500px;
        height : 500px;
    }
</style>