## TP composant 2

1. Créer un composant `popin` dans le module `shared` ;
2. Copier le fichier `shared/popin.component.scss` dans le composant créé ;
3.  Utiliser la *transclusion* avec `<ng-content>` pour injecter le contenu de la popin dans une `div.popin` ;
4. Entourer tous le code de `exercice.component.html` par la balise `<sp-popin></sp-popin>` ;
5. Émettre un événement `exit` si l'utilisateur appuie sur `escape` ou s'il clique à l'extérieure de la `div.popin` ;
6. Écouter l'événement `exit` pour fermer la popin ;