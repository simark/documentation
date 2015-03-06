---
language: Deutsch
currentMenu: install
subTitle: wallabag herunterladen und installieren
---

# wallabag herunterladen und installieren
## Ich möchte wallabag nicht installieren
Wenn du wallabag nicht auf einem eigenen Server installieren kannst oder möchtest, solltest du ein kostenloses Benutzerkonto auf Framabag erstellen, wo wallabag genutzt wird.

## Ich möchte wallabag installieren

[Lade die neueste Version von wallabag herunter](http://www.wallabag.org/download) und entpacke sie. Kopiere die entpackten Dateien und Verzeichnisse auf deinen Webserver.

## Voraussetzungen für den Webserver
* [PHP 5.3.3 oder höher](http://php.net/manual/de/install.php)
* [SQLite](http://php.net/manual/de/book.sqlite.php) oder [MySQL](http://php.net/manual/de/book.mysql.php) oder [PostgreSQL](http://php.net/manual/de/book.pgsql.php)
* [XML for PHP](http://php.net/de/xml)
* [PCRE](http://php.net/de/pcre)
* [Data filtering](http://php.net/manual/de/book.filter.php)
* [Tidy for PHP](http://php.net/de/tidy)
* [cURL](http://php.net/de/curl)
* [allow_url_fopen](http://www.php.net/manual/de/filesystem.configuration.php#ini.allow-url-fopen)
* [gettext](http://php.net/manual/de/book.gettext.php)

Um zu überprüfen, ob dein Server die Voraussetzungen erfüllt, kannst du `wallabag_compatibility_test.php` ausführen. Diese Datei liegt im `install`-Verzeichnis von wallabag.

## Installation der Abhängigkeiten
Damit wallabag ordnungsgemäß funktioniert, müssen einige Abhängigkeiten erfüllt werden. Um diese zu installieren, muss `composer` verwendet werden. Führe folgende Kommandos in deinem wallabag-Verzeichnis aus:

    curl -s http://getcomposer.org/installer | php
    php composer.phar install

Falls du `composer` nicht installieren kannst, kannst du alternativ [vendor.zip](http://wllbg.org/vendor) herunterladen und in deinem wallabag-Verzeichnis entpacken. 

## Berechtigungen
Dein Webserver braucht Schreibrechte in den Verzeichnissen `assets`, `cache`, und `db`. Bei fehlenden Schreibrechten kann die Installation nicht ausgeführt werden.

## wallabag installieren. Endlich.
Rufe wallabag in deinem Browser auf. Wenn dein Server richtig konfiguriert ist, wird die Setup-Seite angezeigt.

Gib dort deinen Datenbank-Typ an (`sqlite`, `mysql` oder `postgresql`) und die Angaben für dein Benutzerkonto

wallabag ist jetzt fertig installiert.

## Anmelden
Rufe wallabag in deinem Webbrowser auf und gib deinen Benutzernamen und dein Passwort ein, um dich anzumelden.

Viel Spaß!
