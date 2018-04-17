## Styles

Il est possible de spécifier directement des styles avec l'attribut *styles*.

Néanmoins, on préfère généralement l'attribut *styleUrls*.

        @Component({
          selector: 'app-generated',
          templateUrl: './generated.component.html',
          styleUrls: ['./generated.component.css']
        })
        export class GeneratedComponent implements OnInit {
        
          constructor() { }
        
          ngOnInit() {
          }
        
        }
