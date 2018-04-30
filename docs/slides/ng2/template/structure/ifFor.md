## NgIf et NgFor

#### ngIf

    <div *ngIf="colors.length > 0">
        <h2>Colors</h2>
    </div>

#### ngFor
    
    <ul>
      <li *ngFor="let color of colors">{{color}}</li>
    </ul>

Variables supplémentaires :

`index`, `even`, `odd`, `first`, `last`

    <ul>
      <li *ngFor="let color of colors; let i = index">{{i}} - {{color}}</li>
    </ul>
