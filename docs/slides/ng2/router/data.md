## data

Il est possible de passer des données de configuration à une route

```
{
  path: 'child',
  component: ChildComponent,
  data: {
    pageTitle: 'Ma page'
  }
}
```

```
constructor( private route: ActivatedRoute ) {}

ngOnInit(){
  this.route.data.subscribe(data => this.pageTitle = data.pageTitle);
  // Ou
  this.page = this.route.snapshot.data.pageTitle;
}
```