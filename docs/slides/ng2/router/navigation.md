## Navigation

Depuis un template HTML, possibilité d'utilisé la directive `routerLink` sur n'importe quelle balise :

```
<div [routerLink]="['/parent', 'child', routeParam]" 
     routerLinkActive="active">...</div>
```

Depuis le code TS avec la méthode `navigate` du router

```
constructor(private router: Router,
            private activatedRoute: ActivatedRoute) {}
...
method() {
  this.router.navigate(['../child'], {relativeTo: this.activatedRoute});
}
```