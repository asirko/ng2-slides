## Sorties

* Entrées = paramètres (parent => l'enfant)
* Sorties = événement (parent <= l'enfant)

```javascript
<app-mon-composant (resultat)="traitement($event)"></app-mon-composant>
```

Pour les événements il faut : le décorateur `@Output()` et un `EventEmitter`

```javascript
@Component({ ... })
export class MonComposant {
  @Output() resultat = new EventEmitter<number>();
  
  emettreScore(): void {
      this.resultat.emit(42);
  }
}
```
