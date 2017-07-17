## Utilisation

```html
<div>
  <app-struct></app-struct>
</div>
```

## Template

```html
<div *ngIf="colors.length > 0">
  <h2>Colors</h2>
  <ul [hidden]="isVisible">
    <li *ngFor="let color of colors; let i = index;">{{i}} - {{color}}</li>
  </ul>
</div>
```
