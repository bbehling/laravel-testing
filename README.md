# Install Laravel Mac

1. Install Virtual Box 6.0
   https://www.virtualbox.org/wiki/Download_Old_Builds
2. Install Vagrant
   https://www.vagrantup.com/

## Install Laravel Homestead per Project

PHP already installed on Mac Catalina

These instructions will install a default Laravel website

1. mkdir projectName & cd projectName
2. Install Composer - download composer install file from https://getcomposer.org/doc/00-intro.md
3. run `php installer`
4. run `php composer.phar create-project --prefer-dist laravel/laravel`
5. cd laravel
6. run `php ../composer.phar require laravel/homestead --dev`
7. run `vendor/bin/homestead make`
8. run `touch ~/.ssh/id_rsa`
9. run `vagrant up`
10. edit host file to forward 192.168.10.10 to homestead.test

## Useful vagrant commands (while in laravel directory with Vagrantfile):

start vagrant vm: `vagrant up`

to ssh into vagrant vm: `vagrant ssh`

delete vargrant vm: `vagrant destroy`

shut down vagrant vm: `vagrant halt`

pause vagrant vm: `vagrant suspend`
