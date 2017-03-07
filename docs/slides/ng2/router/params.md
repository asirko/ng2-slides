# les params

Déclarer une route avec des paramètres :
```
{ path: 'customer/:id', component: DetailComponent }
```

Utilisation dans une page :
```
constructor( private route: ActivatedRoute ) {}

ngOnInit(){
  this.route.params.subscribe(params => {
    let id = +params['id'];
    ...
  });
}

```
