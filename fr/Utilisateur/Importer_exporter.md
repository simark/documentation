---
language: Français
currentMenu: import
subTitle: Importer ou exporter ses données
---

# Importer ou exporter ses données
## Importer

Pour importer des données dans wallabag, vous devez vous rendre dans la page **Configuration**.

### Mise en garde

L'import de données peut être une **opération gourmande** pour votre serveur. C'est pourquoi elle s'effectue en deux étapes :

* l'insertion des URL dans la base de données de wallabag
* dans un second temps, la récupération, pour chaque article, du contenu complet

Ces deux actions ne peuvent pas être effectuées simultanément, car nous vous donnons la possibilité d'importer des milliers de liens, mais aujourd'hui, wallabag n'a pas les possibilités techniques nécessaires pour effectuer tout ce travail automatiquement.

### Depuis Pocket
#### Exporter ses données depuis Pocket

Depuis votre compte Pocket, rendez-vous dans vos options. Depuis là, allez sur la page d'export et cliquez sur le lien *Export HTML file*.

#### Importer ses données Pocket

Depuis la page de configuration de wallabag, partie **Import**, sélectionnez le fichier `ril_export.html` que Pocket a généré puis cliquez sur **Import**.  
wallabag ne fait qu'insérer les liens dans sa base de données. Il faut maintenant lui faire récupérer le contenu de chaque article.

Pour cela, cliquez sur `Click to finish import` : wallabag récupèrera alors le contenu de 10 articles à la fois.

### Depuis Instapaper
#### Exporter ses données depuis Instapaper

Depuis votre compte Instapaper, allez sur la page Settings. Descendez jusqu'à la section Export et exportez en tant qu'HTML. 

#### Importer ses données Instapaper

Sur la page de configuration de wallabag, dans la section **Import**, sélectionnez le fichier `instapaper-export.html` généré par Instapaper, puis cliquez sur **Import**.

### Depuis Readability
#### Exporter ses données depuis Readability

Depuis votre compte Readability, rendez-vous sur la page Tools. Cliquez sur le bouton Export Your Data. Vous recevrez rapidement un courriel à l'adresse électronique liée à votre compte Readability. Ce courriel contient un lien sur lequel vous pouvez télécharger le fichier d'export.

#### Importer ses données Readability

Sur la page de configuration de wallabag, dans la section **Import**, sélectionnez le fichier généré par Readability plus tôt, puis cliquez sur **Import**.

### Depuis wallabag

Puisque vous pouvez exporter vos données de wallabag (lire ci-dessous), il est évidemment possible de les réimporter.

Dans le formulaire d'import, sélectionnez votre fichier d'export wallabag (au format JSON). Démarrez l'import et voila.

Contrairement aux imports ci-dessus, le traitement est moins long car toutes les données (titre et contenu des articles) sont déjà présentes dans le fichier, il n'est pas nécessaire pour wallabag d'accéder à chacune des URL.  
Par contre, le fichier d'import est forcément plus conséquent.

### Depuis vos favoris de navigateur web
wallabag peut importer des données de votre gestionnaire de favoris de votre navigateur, exportées en tant que HTML (Netscape Bookmark File Format).

### Depuis un fichier HTML ou JSON

Si vous avez des entrées au format HTML ou JSON, wallabag devrait être capable de les importer.

## Exporter
Il est possible d'exporter ses données depuis la page **Configuration** de wallabag. Plusieurs raisons possibles :

* réinstaller wallabag
* quitter le service Framabag pour installer soi-même wallabag
* un compte sur un wallabag multi-utilisateurs souhaite avoir sa propre installation de wallabag
* ...

Vous téléchargerez alors un fichier [au format JSON](http://fr.wikipedia.org/wiki/JavaScript_Object_Notation).  
Comme nous l'avons vu ci-dessus, il est possible d'importer ce fichier dans wallabag.
