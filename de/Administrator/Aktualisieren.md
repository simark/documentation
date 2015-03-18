---
language: Deutsch
currentMenu: aktualiseren
subTitle: Aktualisierung
---

# Wallabag aktualisieren
## Eine bestehende Version aktualisieren

 Um deine Installation zu aktualisieren führe folgende Schritte durch: 
 
  1. Lade das Archiv mit der neusten Wallabag Version herunter, beispielsweise mit `wget`.
  1. Entpacke das ZIP-Archiv 
  1. Kopiere die neuen Dateien in das Installationverzeichnis deiner Wallabag-Installation und überschreibe damit die alten Dateien.
  
  Bei einer Debian oder Ubuntu kannst du folgende Befehle benutzen:

      wget http://wllbg.org/latest
      unzip latest
      rsync -ur wallabag-version-number/* /var/www/html/wallabag/ # Der Pfad kann ein anderer sein, etwa /srv/html, /usr/share/nginx/html

Rufe anschließend die Weboberfläche deiner Wallabag-Installation auf und folge den angezeigten Anweisungen um die Aktualisierung abzuschließen.

Am unteren Ende der Konfigurationsseite kannst du überprüfen ob du nun die aktuellste Version benutzt.

###Falls die Aktualisierung scheitert 

Lösche den Ordner `install` und leere den Zwischenspeicher (Cache) mit folgenden Kommandos:

    cd /var/www/html/wallabag/ # ggf. durch eigenen Installationspfad ersetzen
    rm -r cache/* install/

Den Cache kannst du auch auf der Konfigurationsseite leeren. Klicke dort auf den Link "Delete Cache".
