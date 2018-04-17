Pour déclarer une dépendance, il faut l'injecter via le constructeur :

```javascript
@Component({
  selector: 'app-di',
  template:`
    <h1>Dependency injection</h1>
    <ul><li *ngFor="let name of reposNames$ | async">{{name}}</li></ul>
  `
})
export class DiComponent implements OnInit {
  reposNames$: Observable<string>;

  constructor(private githubService: GithubService) {}

  ngOnInit(): void {
    this.reposNames$ = this.githubService.findReposForUser('asirko')
                           .map(repos => repos.map(repo => repo.name));
  }
}
```
