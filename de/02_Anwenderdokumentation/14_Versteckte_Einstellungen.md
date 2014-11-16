## Vorsicht!
Dieser Teil ist nur für fortgeschrittene Anwender. 
**Solltest du beim Bearbeiten einer der Dateien etwas falsch machen, kann es sein, dass wallabag nicht mehr funktioniert.**
Es muss eine wichtige Datei von wallabag bearbeitet werden, `inc/poche/config.inc.php`, deshalb mache unbedingt eine Sicherungskopie dieser Datei, bevor du etwas änderst!

Die Datei wird während der Installation von wallabag erzeugt und mit Standardeinstellungen initialisiert. Durch Anpassen der Datei kann das Verhalten von wallabag in einigen Punkten angepasst werden, die nicht über die nicht über der Konfigurationsseite verfügbar sind.

## Fortgeschrittene Einstellungen

Jeder der in `inc/poche/config.inc.php` definierten Parameter ist folgendermaßen angegeben:

    @define ('PARAMETER_NAME', 'Parameter-Wert');
    
Es darf in jeder Zeile ausschließlich `Parameter-Wert` geändert werden. 
Ändere keine anderen in der Datei angegebenen Parameter!

Änderbare Parameter: 

|PARAMETER_NAME|Standardwert|Beschreibung|erwarteter Wert|
|---|---|---|:---:|
`HTTP_PORT`         | `80`| entspricht dem HTTP-Port auf deinem Webserver. Nur ändern, wenn sich dein Web-Server hinter einem Proxy befindet. | ganze Zahl|
|`SSL_PORT`         | `443`| entspricht dem SSL-Port auf deinem Webserver. Ändern, wenn du sslh verwendest.| ganze Zahl|
|`DEBUG_POCHE`      | `FALSE`| Wenn du Probleme mit wallabag hast, kann es bei der Fehlersuche helfen, den Debug-Modus zu aktivieren. | `TRUE` / `FALSE`|
|`DOWNLOAD_PICTURES`| `FALSE`| Damit kannst du Bilder aus Artikeln herunterladen (zusätzlich zum Artikeltext). Diese Einstellung ist standardmäßig deaktiviert, um eine Überlastung des Webservers zu vermeiden. Wir bevorzugen, dich diese Einstellung selbst aktivieren zu lassen. | `TRUE` / `FALSE`|
|`SHARE_TWITTER`    | `TRUE`| ermöglicht die gemeinsame Nutzung mit Twitter | `TRUE` / `FALSE`|
|`SHARE_MAIL`       | `TRUE`| ermöglicht den Austausch per E-Mail | `TRUE` / `FALSE`|
|`SHARE_SHAARLI`    | `FALSE`| ermöglicht die gemeinsame Nutzung mit einer Shaarli-Installation (ein Lesezeichen-Manager) | `TRUE` / `FALSE`|
|`SHAARLI_URL`      | `'http://myshaarliurl.com'`| Definiert die URL Ihrer Installation Shaarli.| URL|
|`FLATTR`           | `TRUE`| Aktiviert die Möglichkeit, einen Artikel zu flattrn ([Flattr ist eine Plattform für Mikrospenden] (http://de.wikipedia.org/wiki/Flattr)). Wenn ein Artikel flattrbar ist, wird ein Symbol angezeigt und ermöglicht es, eine Mikro-Spende an den Autor des Artikels zu senden. | `TRUE` / `FALSE`|
|`SHOW_PRINTLINK`   | `'1'`| Zeigt eine Link, um einen Artikel zu drucken. | `'0'` (deaktiviert), `'1'` (aktiviert)|
|`SHOW_READPERCENT` | `'1'`| Zeige den bereits gelesenen Anteil im Artikel (nur bei den Themes `default`, `dark`, `dmagenta`, `solarized`, `solarized-dark`). | `'0'` (deaktiviert), `'1'` (aktiviert)|
|`PAGINATION`       | `'12'`| Definiert die Anzahl der Einträge, die auf einer Seite dargestellt werden. | ganze Zahl|
