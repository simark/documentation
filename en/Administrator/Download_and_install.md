---
language: English
currentMenu: install
subTitle: Download and install wallabag
---

# Download and install wallabag
## I don't want to install wallabag

If you can't or don't want to install Wallabag on your server, we suggest you create a free account on [Framabag](https://framabag.org/) wich uses our software: read the complete documentation here (TODO write Create a framabag account).

## I want to install wallabag

### I want to download wallabag the easiest way possible

[Download the latest wallabag version](http://wllbg.org/latest) and unpack it. Copy the files on your web server. Jump off to next section.

### I want to download wallabag via composer

You need to install composer: 

    curl -s http://getcomposer.org/installer | php

Next, on your web server, run this command: 

    composer create-project wallabag/wallabag . dev-master

All is downloaded into `wallabag` folder.

### Permissions

Your web server needs a writing access to the `assets`, `cache` and `db` directories. Otherwise, a message will report that the installation is impossible.

### Installation of wallabag. At last.

Access to wallabag from your web browser. If your server is correctly configured, you directly reach the setup screen. 

#### Prerequisites
The installer will tell you which prerequisites are missing. If there's any, jump off to the [corresponding session](#Prerequisites) to know how to deal with that problem.

#### Twig installation
wallabag is build with Twig, a template library. You have to download it for wallabag to work.
* One option is to choose the automatic download of the package which will be automatically downloaded and installed.
* If this option fails, you can choose the second option which is to manually download [the vendor package](http://wllbg.org/vendor), unzip it and copy the vendor directory in your wallabag directory
* Finally, you can here also use Composer to install Twig by following the commands written on screen :

    ```
    curl -s http://getcomposer.org/installer | php
    php composer.phar install
    ```

#### Database connection
You have to choose a database system between :
* **SQLite** : The easiest system of all. No extra configuration needed.
* **MySQL** : A well known database system, which is in most cases more efficient than SQLite
* **Postgresql** : Some people found it better than MySQL.

*Note :* If you're using MySQL or Postgresql, you have to **fill all the fields**, otherwise the installation will not work and an error message will tell you what's wrong. You must create the database that you will use for wallabag manually with a tool like PHPMyAdmin or the console.

#### User Account
Finally, you need to create an user account. As always, be sure to choose a strong password.
An email field is present but it is not at all required.

If you get a green success message, it means wallabag is now installed.

### <a name="Prerequisites"></a>Prerequisites
#### List of prerequisites for your web server

* [PHP 5.3.3 or more](http://php.net/manual/en/install.php) **with [PDO](http://php.net/manual/en/book.pdo.php) support**
* [SQLite](http://php.net/manual/en/book.sqlite.php) **or** [MySQL](http://php.net/manual/fr/book.mysql.php) **or** [PostgreSQL](http://php.net/manual/en/book.pgsql.php)
* [XML for PHP](http://php.net/xml)
* [PCRE](http://php.net/pcre)
* [ZLib](http://php.net/zlib)
* [mbstring](http://php.net/mbstring) and/or [iconv](http://php.net/iconv)
* The [DOM/XML](http://php.net/manual/en/book.dom.php) extension
* [allow_url_fopen](http://www.php.net/manual/en/filesystem.configuration.php#ini.allow-url-fopen)
* [gettext](http://php.net/manual/en/book.gettext.php)

Optionnal :
* [cURL](http://php.net/curl) (with Parallel URL fetching) or [allow_url_fopen](http://www.php.net/manual/en/filesystem.configuration.php#ini.allow-url-fopen)
* [GD](http://php.net/manual/en/book.image.php)
* [Data filtering](http://php.net/manual/book.filter.php)


## Login

From your web browser, you reach the login screen: fill your username and your password to connect to your account.

Enjoy!
