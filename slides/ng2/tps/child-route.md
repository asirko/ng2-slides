## TP filiation de routes

    git checkout exo-childRoute
1.  Dans `stat-routing.module.ts` :
   1. créer 2 routes enfants (`synthesis` et `graph`) qui affiche respectivement `SynthesisComponent` et `GraphComponent`;
   2. dans ses routes enfants, ajouter une redirection de la route `''` vers le chemin `synthesis` ;
2. Dans `visualization.component.html` :
   1. ajouter l'outlet à la fin du fichier ;
   2. transformer les 2 `option` en lien vers les 2 nouvelles routes ;
   3. la route active doit avoir la classe `active`.