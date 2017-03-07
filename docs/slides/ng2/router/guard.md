# Guard
4 contrôles possibles sur la navigation :
- CanActivate : valide l'accès à la route
- CanActivateChild : valide l'accès aux enfants de la route
- CanDeactivate - Decides if a route can be deactivated
- CanLoad - Decides if a module can be loaded lazily

```
{ path: '', component: UnComposant, canActivate: ['MonGuard'] }
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
