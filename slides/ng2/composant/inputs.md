## Entrées

On peut passer des données à un composant enfant :
```javascript
...
<app-mon-composant [nbJeux]="3"></app-mon-composant>
...
```

Pour ça, il faut utiliser le décorateur `@Input()`

```javascript
@Component({
    selector: 'app-mon-composant',
    ...
})
export class MonComposant implements OnInit {
  @Input() nbJeux: number;
  constructor () {
      console.log(this.nbJeux); // => undefined
  }
  ngOnInit(): void {
      console.log(this.nbJeux); // => 3
  }
}
```
