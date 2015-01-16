---
language: English
currentMenu: vagrant
subTitle: Vagrant
---

# Vagrant

In order to allow you to easily set up the required configuration for wallabag, we offer you a Vagrantfile file to be used with [Vagrant](http://www.vagrantup.com).

[According to Wikipedia,](https://en.wikipedia.org/wiki/Vagrant_%28software%29)

    Vagrant is computer software for creating and configuring virtual development environments. It can be seen as a wrapper around virtualization software such as VirtualBox, KVM, VMware and around configuration management software such as Ansible, Chef, Salt or Puppet.

## Use Vagrant for wallabag

Here is the procedure to run wallabag inside a Vagrant container:

    wget -O wallabag-dev.zip https://github.com/wallabag/wallabag/archive/dev.zip
    unzip wallabag-dev.zip
    cd wallabag-dev
    vagrant up

Now, go to `http://localhost:8003`, wallabag should be available there! (make sure you do not use the port 8003 of your machine for something else before)

## What did the Vagrantfile install ?

The script install a LAMP server, i.e. :

* Ubuntu 14.04
* an Apache2 web server
* PHP5
* SQLite or MySQL or PostgreSQL for PHP
* XDebug for PHP
