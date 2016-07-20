# PHP Utilities 

## Composer :

#### Download Composer :

```bash
$ curl https://getcomposer.org/composer.phar
```

#### Alias Linux

```bash
$ curl -sS https://getcomposer.org/installer | php
$ sudo mv composer.phar /usr/local/bin/composer
```
## Frameworks :

#### Symfony :

+ Start server 

    + SF 3 or + :
    ```bash
    $ php bin/console server:run +options
    ```
    +  SF 2 :
    ```bash
    $ php app/console server:run +options
    ```

+ Update database : 

    + SF 3 or + :
    ```bash
    $ php bin/console doctrine:schema:update --force
    ```
    +  SF 2 :
    ```bash
    $ php app/console doctrine:schema:update --force
    ```
    
#### ZendFramework :

+ Start server :

```bash
$ cd path/to/install
$ php -S 0.0.0.0:8888 -ddisplay_errors=0 -t public public/index.php
```

+ Development mode :

```bash
$ cd path/to/install
$ php public/index.php development enable 
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
