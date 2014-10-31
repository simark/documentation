## I don't want to install Wallabag
If you can't or don't want to install Wallabag on your server, we suggest you create a free account on Framabag wich uses our software: read the complete documentation here (TODO write Create a framabag account).

## I want to install Wallabag
 
[Download the latest wallabag version](http://www.wallabag.org/download) and unpack it. Copy the files on your web server.

## Prerequisites for your web server
* [PHP 5.3.3 or more](http://php.net/manual/en/install.php)
* [SQLite](http://php.net/manual/en/book.sqlite.php) or [MySQL](http://php.net/manual/fr/book.mysql.php) or [PostgreSQL](http://php.net/manual/en/book.pgsql.php)
* [XML for PHP](http://php.net/xml)
* [PCRE](http://php.net/pcre)
* [Data filtering](http://php.net/manual/book.filter.php)
* [Tidy for PHP](http://php.net/tidy)
* [cURL](http://php.net/curl)
* [allow_url_fopen](http://www.php.net/manual/en/filesystem.configuration.php#ini.allow-url-fopen)
* [gettext](http://php.net/manual/en/book.gettext.php)

To ensure that your server has all the prerequisites, you can run the file `wallabag_compatibility_test.php` that is located in the `install` directory of wallabag.

## Installation of the dependencies 
In order to work properly, wallabag needs some dependencies. To install them, you have to use `composer`. In your wallabag folder, run the following commands:

    curl -s http://getcomposer.org/installer | php
    php composer.phar install

If you can't install `composer` (In order to work properly, Wallabag needs some dependencies), we provide you a [vendor.zip](http://wllbg.org/vendor) file to unpack in your wallabag directory. 

## Permissions
Your web server needs a writing access in `assets`, `cache` and `db` directory. Otherwise, a message will report that the installation is impossible.

## Installation of wallabag. At last.
Access to wallabag from your web browser. If your server is correctly configured, you reach the setup screen.  

Fill your database type (`sqlite`, `mysql` ou `postgresql`) and finally the information for your user account.

wallabag is now installed. 

## Login 

From your web browser, you reach the login screen : fill your username and your password to connect to your account.

Enjoy!