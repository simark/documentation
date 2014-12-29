---
language: English
currentMenu: upgrade
subTitle: Update wallabag
---

## Update an existing wallabag installation

 In order to update your installation, download and unzip the archive into your installation folder. For example on Ubuntu/Debian:

    wget http://wllbg.org/latest
    unzip latest
    rsync -ur wallabag-version-number/* /var/www/html/wallabag/

Delete the `install folder and clear the cache:

    cd /var/www/html/wallabag/
    rm -r cache/* install/

Clearing the cache is also possible in the configuration page, clicking on the link `Delete Cache.

Verify at the bottom of the configuration page that you're running the last version.
