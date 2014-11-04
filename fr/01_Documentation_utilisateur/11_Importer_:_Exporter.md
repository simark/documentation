## Importer
Pour importer des données dans wallabag, vous devez vous rendre dans la page **Configuration**. 

### Mise en garde
L'import de données peut être une **opération gourmande** pour votre serveur.

### Depuis Pocket
TODO

### Depuis Instapaper
TODO

### Depuis Readability
TODO

### Depuis wallabag
Puisque vous pouvez exporter vos données de wallabag (lire ci-dessous), il est évidemment possible de les réimporter. 

Dans le formulaire d'import, sélectionnez votre fichier d'export wallabag (au format JSON). Démarrez l'import et voila. 

Contrairement aux imports ci-dessus, le traitement est moins long car toutes les données (titre et contenu des articles) sont déjà présentes dans le fichier, il n'est pas nécessaire pour wallabag d'accéder à chacune des URL.  
Par contre, le fichier d'import est forcément plus conséquent. 

### Depuis un fichier HTML ou JSON
TODO

## Exporter
Il est possible d'exporter ses données depuis la page **Configuration** de wallabag. Plusieurs raisons possibles : 
* réinstaller wallabag
* quitter le service Framabag pour installer soi-même wallabag
* un compte sur un wallabag multi-utilisateurs souhaite avoir sa propre installation de wallabag
* ...

Vous téléchargerez alors un fichier [au format JSON](http://fr.wikipedia.org/wiki/JavaScript_Object_Notation).  
Comme nous l'avons vu ci-dessus, il est possible d'importer ce fichier dans wallabag. 