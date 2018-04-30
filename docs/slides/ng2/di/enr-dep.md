Pour enregistrer une dépendance : 

    @NgModule({
      declarations: [],
      imports: [],
      providers: [GithubService],
      bootstrap: [AppComponent]
    })
    export class AppModule {
    }

Il faut qu'elle soit déclarée comme injectable&nbsp;:

```javascript
@Injectable()
export class GithubService {
    
}
```
