## TP RxJS et HTTP

    git checkout exo-obs
1. Dans le composant `synthesis.component.ts`, compléter toutes les méthodes et logguer leurs résultats depuis la méthode ngOnInit ;
2. Dans le composant `stat.component.ts` gérer le redimensionnement du graphique :
   - l'événement `mousedown` sur le `separator` déclanche le mouvement ;
   - à chaque `mousemove` qui suit , redimentionner les deux blocs et notifier le `resizeGraphService` du nouvel espace dans le bloc de droite ;
   - arréter d'écouter `mousemove` sur l'événement `mouseup` ;