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

forRoot pour le Root Module et forChild pour tous les autres
