## Operateurs sur les obervables

* un événement transmis par un observable est un objet
* cet objet qui transite peut être transformer avant sa consomation par le subscribe
* __beaucoup d'opérateurs de transformation possible__
* les transformations s'applique avec `pipe()`

```javascript
let childNames = [];
users$.pipe(
    filter(u => u.age < 18),
    map(child => child.name)
).subscribe(childName => childNames.push(childName))
```
