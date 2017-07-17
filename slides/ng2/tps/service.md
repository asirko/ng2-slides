## Exemple de Service : le Store

* c.f. : `record-store.service.ts` :
  * Stock un `Record` temporairement pour le mettre à disposition de tous ceux qui le veulent ;
  * Utilise le `BeheaviorSubject` ;
* c.f. : `http-auth.service.ts` :
  * surcharge les méthode du service HTTP d'Angular
  * ajoute le token si nécessaire ;
  * redirige à l'accueil s'il n'y a pas de token
