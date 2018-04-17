## Number

Permet de formatter un nombre

Le format dépend de la local de l'application 
(possibilité de changer la local dans l'application)

Prend un seul param sous la forme : `{integerDigits}.{minFractionDigits}-{maxFractionDigits}`

        <p>{{ 12345 | number }}</p> <!-- 12 345 -->
        <p>{{ 12345 | number:'9.' }}</p> <!-- 000 012 345 -->
        <p>{{ 12345 | number:'.2' }}</p> <!-- 12 345,00 -->
        <p>{{ 12345.14 | number:'.1-1' }}</p> <!-- 12 345,1 -->
        <p>{{ 12345.16 | number:'.1-1' }}</p> <!-- 12 345,2 -->
