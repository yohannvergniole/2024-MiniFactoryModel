---
layout: default
nav_order: 8
title: Charnière
parent: Études et choix techniques
---

<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.4.0/model-viewer.min.js"></script>

Étant donné que nous avons besoin qu'un côté de la mallette soit pliable, nous avons besoin d'un mécanisme permettant de le faire. Nous avons donc opté pour une charnière piano sur toute la longueur de la mallette.


<model-viewer
    class="viewer"
    alt="Modèle 3D de l'armature"
    src="../shared-assets/models/hinge.gltf"
    poster="../shared-assets/images/capture_charniere.png"
    shadow-intensity="1"
    camera-controls
    touch-action="pan-z"
    rotation="90 90 90">
</model-viewer>

<style>
    .viewer
    {
        margin : auto;
        width : 500px;
        height : 500px;
    }
</style>

Nous pouvons ainsi la fixer sur notre mallette. Cependant, cette charnière nous inflige une nouvelle contrainte. En effet, à cause de celle-ci, nous ne pouvons pas fixer notre armature sur les bords de nos planches de peuplier : les profilés faisant 20mm et la charnière faisant 32mm (donc 16mm de chaque côté), il est impossible de fixer notre charnière sur nos planches. Nous avons donc décider de décaler l'armature comme ceci :
<model-viewer
    class="viewer"
    alt="Modèle 3D de l'armature"
    src="../shared-assets/models/problemeCharniere.gltf"
    poster="../shared-assets/images/problemeCharniere.png"
    shadow-intensity="1"
    camera-controls
    touch-action="pan-z"
    rotation="90 90 90">
</model-viewer>

Malheureusement pour nous, ceci créé un autre problème. Visser la charnière seulement dans une plaque de 5mm met en péril la solidité de la structure. Nous avons donc besoin d'une [pièce de support](../realisation/ressources.md#les-profilés) dans laquelle nous allons visser la charnière.
