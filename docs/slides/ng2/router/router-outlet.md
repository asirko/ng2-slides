## router-outlet

Le composant de la route est placé dans le `router-outlet`.

```
<sp-header></sp-header>

<div class="content">
  <router-outlet></router-outlet>
</div>
```

Il est possible d'avoir plusieurs `router-outlet` :
- inclu les uns dans les autres (filiation de routes) ;
- de même niveau en les nommant (routage parallèle) => [named outlet](http://onehungrymind.com/named-router-outlets-in-angular-2/)