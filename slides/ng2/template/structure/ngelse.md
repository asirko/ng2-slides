## ngIf / else

```
<div *ngIf="colors.length > 0; else noColors">
    <h2>Colors</h2>
</div>
<ng-template #noColors>
    <div>No colors</div>
</ng-template>
```