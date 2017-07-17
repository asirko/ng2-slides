## Resolver

Permet de récupérer certaines données côté serveur avant d'afficher la nouvelle route.

Un `resolver` est un service qui implémente `Resolve<T>` :

```
resolve(route: ActivatedRouteSnapshot, state: RouterStateSnapshot)
		: Observable<T> | Promise<T> | T
```

```
{ 
  path: 'child',
  component: ChildComponent,
  resolve: {
    result: myResolver
  }
}
```
Ici `result` est le nom de la valeur une fois résolue, elle sera ajoutée à l'objet data (vu avant)