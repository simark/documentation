---
language: Français
currentMenu: install
subTitle: Télécharger et installer wallabag
---

## Je ne souhaite pas installer wallabag

Puisque vous ne voulez pas, puisque vous ne pouvez pas, nous vous proposons de vous créer un compte gratuit : [lisez la documentation complète ici](Utilisateur/Framabag.md).

## Je souhaite installer wallabag

[Téléchargez la dernière version de wallabag](http://wllbg.org/latest) et décompressez-la :

    wget http://wllbg.org/latest
    unzip latest
    mv wallabag-version-number wallabag

Copiez les fichiers sur votre serveur web. Dans le cas d'Ubuntu/Debian, il s'agit de /var/www/html/ :

    sudo mv wallabag /var/www/html/

### Pré-requis pour votre serveur web

* [PHP 5.3.3 ou plus](http://php.net/manual/en/install.php)
* [SQLite](http://php.net/manual/en/book.sqlite.php) ou [MySQL](http://php.net/manual/fr/book.mysql.php) ou [PostgreSQL](http://php.net/manual/en/book.pgsql.php)
* [XML pour PHP](http://php.net/xml)
* [PCRE](http://php.net/pcre)
* [Filtrage des données](http://php.net/manual/book.filter.php)
* [Tidy pour PHP](http://php.net/tidy)
* [cURL](http://php.net/curl)
* [allow_url_fopen](http://www.php.net/manual/en/filesystem.configuration.php#ini.allow-url-fopen)
* [gettext](http://php.net/manual/en/book.gettext.php)

Pour être sûr que votre serveur possède tous les pré-requis, vous pouvez exécuter le fichier `wallabag_compatibility_test.php` qui se trouve dans le répertoire `install` de wallabag : dans votre navigateur, accédez à `http://votreserveur.com/wallabag/install/wallabag_compatibility_test.php` et installez les composants requis. Par exemple pour Tidy sur Ubuntu/Debian :

    sudo apt-get install php5-tidy
    sudo service apache2 reload

### Installation des dépendances

Pour pouvoir fonctionner, wallabag a besoin de dépendances. Pour les installer, vous devez utiliser `composer`. Placez-vous dans votre dossier wallabag (toujours dans le cas d'Ubuntu/Debian : <code>/var/www/html/wallabag/</code>) et exécutez les commandes suivantes :

    curl -s http://getcomposer.org/installer | php
    php composer.phar install

Si vous ne pouvez pas installer `composer` (dans le cas d'hébergement mutualisé par exemple), nous vous proposons un fichier [vendor.zip](http://wllbg.org/vendor). Vous pouvez soit le télécharger puis le décompresser dans votre répertoire wallabag, soit laisser le script d'installation le faire pour vous.

### Création de la base de données MySQL

wallabag peut s'installer sur différents types de bases de données (`sqlite`, `mysql` ou `postgresql`), mais nous vous conseillons d'utiliser MySQL, plus performante. Il est alors nécessaire de créer une nouvelle base (par exemple `wallabag`) , un nouvel utilisateur (par exemple  `wallabag`) et un mot de passe (ici `VotreMotdePasse`). Vous pouvez pour cela utiliser 'phpMyAdmin', ou exécuter les commandes suivantes :

    mysql -p -u root
    mysql> CREATE DATABASE wallabag;
    mysql> GRANT ALL PRIVILEGES ON `wallabag`.* TO 'wallabag'@'localhost' IDENTIFIED BY 'VotreMotdePasse';
    mysql> exit

### Permissions

Le serveur web doit avoir accès en écriture aux répertoires `assets`, `cache` et `db`. Sans cela, un message vous indiquera que l'installation est impossible :

    sudo chown -R www-data:www-data /var/www/html/wallabag

### Installation de wallabag. Enfin.

Accédez à wallabag depuis votre navigateur : `http://votreserveur.com/wallabag`. Si votre serveur est bien configuré, vous arrivez sur l'écran d'installation.

Renseignez le type de votre base de données (`sqlite`, `mysql` ou `postgresql`) et les informations de votre base de données. Dans le cas de la base MySQL créée plus haut, la configuration standard sera :

    Database engine:    MySQL
    Server:             localhost
    Database: 	        wallabag
    Username:	        wallabag
    Password:	        VotreMotdePasse

Créez enfin votre premier utilisateur et son mot de passe (différents de l'utilisateur de la base de données).

wallabag est maintenant installé.

## Connexion

Vous arrivez sur l'écran d'identification : saisissez votre identifiant et votre mot de passe et vous voici connecté.