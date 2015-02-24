paunin/sf2_vagrant
====================

# Overview

* Vagrant with ansible provisioning
* Symfony 2 with set of bundles for work with rabbitMQ and admin CRUD panel

# Requirements

* [Ansible](http://ansible.com)
* [Vagrant](https://www.vagrantup.com/)

# Install

* Up vagrant `vagrant up --provision`
* Go to vagrant box `vagrant ssh`
* Go to doc root `cd /var/www`
* Run `php composer.phar install -vv`  from project directory or `php composer.phar update -vv`
* Install DB schema `php app/console doctrine:schema:update --force`
* Load fixtures `php app/console doctrine:fixtures:load`
    
# Run

## Application

Open [http://sf2.virtual.local:8080/app_dev.php](http://sf2.virtual.local:8080//app_dev.php) or [http://localhost:8888/app_dev.php](http://localhost:8888/app_dev.php)

## RabbitMQ panel

Open [http://sf2.virtual.local:15672](http://sf2.virtual.local:15672) or [http://localhost:15673](http://localhost:15673)
