## Я не хочу устанавливать wallabag
Если вы не хотите или не можете установить Wallabag на свой сервер, мы предлагаем вас создать бесплатный аккаунт на Framabag, где используется наше программное обеспечение: прочитайте об этом здесь (TODO написать Создание аккаунта framabag).

## Я хочу установить wallabag
 
[Скачайте последнюю версию wallabag](http://www.wallabag.org/download) и распакуйте её. Скопируйте файлы на свой веб-сервер.

## Требования к вашему веб-серверу
* [PHP 5.3.3 or more](http://php.net/manual/en/install.php)
* [SQLite](http://php.net/manual/en/book.sqlite.php) или [MySQL](http://php.net/manual/fr/book.mysql.php) или [PostgreSQL](http://php.net/manual/en/book.pgsql.php)
* [XML for PHP](http://php.net/xml)
* [PCRE](http://php.net/pcre)
* [Data filtering](http://php.net/manual/book.filter.php)
* [Tidy for PHP](http://php.net/tidy)
* [cURL](http://php.net/curl)
* [allow_url_fopen](http://www.php.net/manual/en/filesystem.configuration.php#ini.allow-url-fopen)
* [gettext](http://php.net/manual/en/book.gettext.php)

Чтобы убедиться, что ваш веб-сервер удовлетворяет всем требованиям, вы можете запустить файл `wallabag_compatibility_test.php`, который находится в подпапке `install` в основной папке wallabag.

## Установка зависимостей
Для корректной работы wallabag нужно установить несколько зависимостей. Чтобы сделать это, вы должны использовать `composer`. Перейдите в папку с wallabag и запустите следующие команды:

    curl -s http://getcomposer.org/installer | php
    php composer.phar install

Если вы не можете установить `composer` (для корректной работы wallabag нужно установить несколько зависимостей), мы предлагаем распаковать файл [vendor.zip](http://wllbg.org/vendor) в вашей папке wallabag. 

## Разрешения
Вашему серверу нужен доступ для записи в папках `assets`, `cache` и `db`. В противном случае появится сообщение о невозможности установки.

## Установка wallabag. Наконец-то.
Зайдите на сайт с wallabag из вашего браузера. Если сервер настроен правильно, вы увидите страницу установки.

Укажите тип вашей базы данных (`sqlite`, `mysql` или `postgresql`) и, наконец, информацию для вашего аккаунта.

Теперь wallabag установлен.

## Вход в wallabag

В вашем браузере откроется страница входа: введите своё имя пользователя и пароль для доступа к своему аккаунту.

Пользуйтесь!
