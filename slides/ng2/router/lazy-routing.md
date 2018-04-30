## Lazy loading


```
{ 
  path: 'profile', 
  loadChildren: 
  'app/profile/profile.module#ProfileModule' 
}
```
```
[
  {path: '', component: ListComponent}, 
  {path: ':id', component: DetailComponent }
]
```
=> Scope les routes de profile derrière la route `/profile`
