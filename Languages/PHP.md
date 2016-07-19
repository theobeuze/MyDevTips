# PHP Utilities 

## Composer :

#### Alias Linux

```bash
$ curl -sS https://getcomposer.org/installer | php
$ sudo mv composer.phar /usr/local/bin/composer
```

## Server :

#### Switch PHP Version 

+ From php5.6 to php7.0 :

*Apache:*
```bash
$ sudo a2dismod php5.6 
$ sudo a2enmod php7.0
$ sudo service apache2 restart
```
*CLI:*
```bash
$ sudo ln -sfn /usr/bin/php7.0 /etc/alternatives/php
```

+ from php7.0 to php5.6:

*Apache:*
```bash
$ sudo a2dismod php7.0
$ sudo a2enmod php5.6 
$ sudo service apache2 restart
```
*CLI:*
```bash
$ sudo ln -sfn /usr/bin/php5.6 /etc/alternatives/php
```


#### Server PHP

+ Run server with Xdebug and Display Errors :

```bash
$ php -S localhost:8080 -dzend_extension=xdebug.so -dxdebug.remote_autostart=1 -display_errors=1
```
