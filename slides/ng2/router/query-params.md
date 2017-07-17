## Les query params

Naviguer avec des query params :
```
<a [routerLink]="['/']" [queryParams]="{ page: 99 }">Page 99</a>
```
```
goToPage(pageNum) {
    this.router.navigate(['/product-list'], { queryParams: { page: pageNum } });
  }
```

Récupérer les paramètres :

```
constructor( private route: ActivatedRoute ) {}

ngOnInit(){
  this.route.queryParams.subscribe(params => this.page = param.page);
  // Ou
  this.page = this.route.snapshot.queryParams.page;
}
```
