## Filiation de route

```
Routes = [{
  path: 'parent',
  component: ParentComponent,
  children: [{
    path: 'child',
    component: ChildComponent
  }]
}];
```

Implique que `parent.component.html` contienne un `router-outlet`:

```
<div>
  <div class="nav">...</div>
  <router-outlet></router-outlet>
</div>
```