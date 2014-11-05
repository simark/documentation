## Vorsicht!
**Achtung**, dieser Teil ist nur für fortgeschrittene Anwender. wir werden eine wichtige Datei von wallabag bearbeiten, `inc/poche/config.inc.php`, deshalb mache bitte eine Sicherungskopie dieser Datei, bevor du etwas änderst!
**Solltest du beim Bearbeiten einer der Dateien etwas falsch machen, kann es sein, dass wallabag nicht mehr funktioniert.**

Die Datei wird während der Installation von wallabag erzeugt.
Also: wallabag installieren, eine Sicherungskopie von `inc/poche/config.inc.php` machen und die Originaldatei mit deinem bevorzugten Texteditor öffnen.

In dieser Datei sind einige Parameter definiert, die nicht über die nicht auf der Konfigurationsseite einstellbar sind.

## Fortgeschrittene Einstellungen

Jeder dieser Parameter ist folgendermaßen angegeben:

    @define ('PARAMETER_NAME', 'Parameter-Wert');
    
Es darf in jeder Zeile ausschließlich `Parameter-Wert` geändert werden. 

TODO explain all the following parameters

Änderbare Parameter: 
* `HTTP_PORT` (Standardwert ist `80`): erwarteter Wert: eine ganze Zahl.
* `SSL_PORT` (Standardwert ist `443`): erwarteter Wert: eine ganze Zahl. 
* `DEBUG_POCHE` (Standardwert ist `FALSE`): erwarteter Wert: `TRUE` oder `FALSE`.
* `DOWNLOAD_PICTURES` (Standardwert ist `FALSE`): erwarteter Wert: `TRUE` oder `FALSE`.
* `SHARE_TWITTER` (Standardwert ist `TRUE`): erwarteter Wert: `TRUE` oder `FALSE`.
* `SHARE_MAIL` (par défaut, `TRUE`): erwarteter Wert: `TRUE` oder `FALSE`.
* `SHARE_SHAARLI` (Standardwert ist `FALSE`): erwarteter Wert: `TRUE` oder `FALSE`.
* `SHAARLI_URL` (Standardwert ist `'http://myshaarliurl.com'`): erwarteter Wert: deine Shaarli URL. 
* `FLATTR` (Standardwert ist `TRUE`): erwarteter Wert: `TRUE` oder `FALSE`.
* `SHOW_PRINTLINK` (Standardwert ist `'1'`): erwarteter Wert: `'0'` zum deaktivieren, `'1'` zum aktivieren.
* `SHOW_READPERCENT` (Standardwert ist `'1'`): erwarteter Wert: '0'` zum deaktivieren, `'1'` zum aktivieren.
* `PAGINATION` (Standardwert ist `'12'`): erwarteter Wert: eine ganze Zahl. 
