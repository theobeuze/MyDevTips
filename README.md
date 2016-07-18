# PHP Utilities 

## Switch PHP Version 

+ From php5.6 to php7.0 :
Apache:
sudo a2dismod php5.6 ; sudo a2enmod php7.0 ; sudo service apache2 restart
CLI:
sudo ln -sfn /usr/bin/php7.0 /etc/alternatives/php

+ from php7.0 to php5.6:
Apache:
sudo a2dismod php7.0 ; sudo a2enmod php5.6 ; sudo service apache2 restart
CLI:
sudo ln -sfn /usr/bin/php5.6 /etc/alternatives/php
