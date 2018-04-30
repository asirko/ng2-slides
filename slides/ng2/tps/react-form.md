## TP formulaires

```
git checkout exo-form
```

Dans le composant `exercice.component.ts`

1. créer le `formGroup` dans la méthode `ngOnInit` puis lier le formGroup et ses champs au template ;
2. si la `category` change, vider le formulaire ;
3. ajouter une validation inter champs au formGroup (cf: `TODO: validation`) ;
4. ajouter un `Output` d'`Exercice` , `addExercice` émet la valeur si le formulaire est valide et `close` émet `null` ;
5. la méthode `getTitle` renvoit les erreurs formattées ;
6. **facultatif :** faire une saisie assisté pour le champ `type` (liste des suggestions disponibles dans `Exercice.ts`).