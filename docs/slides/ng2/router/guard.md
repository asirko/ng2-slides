## Guard

4 contrôles possibles sur la navigation :
- CanActivate : valide l'accès à la route
- CanActivateChild : valide l'accès aux enfants de la route
- CanDeactivate : valide que l'on a le droit de quitter la route
- CanLoad : valide que l'on peut charger la route en lazy loading

```
{ path: '', component: ChildComposant, canActivate: ['MonGuard'] }
```

```
@Injectable()
export class MonGuard implements CanActivate {
  constructor(private authService: AuthService) {}
  canActivate() {
    return this.authService.isLoggedIn();
  }
}
```
