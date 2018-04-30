# déclaration

déclaration dans les modules, exemple :

 ```javascript
 const routes: Routes = [
   {
     path: '',
     redirectTo: '/home',
     pathMatch: 'full'
   },
   { path: 'home', component: HomeComponent },
   { path: '**', component: Erreur404Component }
 ];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }
 ```

1 route = 1 composant (null autorisé)