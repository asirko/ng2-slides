# Binding

* Toutes les propriétés du DOM accessibles
* Sensible à la casse
* Fonctionne avec les webcomponents


```
<div [hidden]="1 === 1">Ce texte sera caché</div>
<input type="text" [value]="maVariable">
<input type="radio" [checked]="true">

<!-- ET -->
<h1>{{titre}}</h1>
<!-- équivaut à -->
<h1 [textContent]="titre"></h1>
``` 

