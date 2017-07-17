- Faire fonctionner le filtre des Stats :
   1. créer le pipe dans `share/exercice` ;
   2. le pipe renvoit une sous liste de record correspondant auparamètre `category` ;
   3. l'utiliser dans `SelectorComponent` :
      1. le switch permet de selectionner une `category` ;
      2. le bouton sélectionné est mis en valeur avec la classe `active`;
      3. utiliser la valeur séléctionnée pour filtrer les `records`