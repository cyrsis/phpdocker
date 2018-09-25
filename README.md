
# phpdocker

September 25, 2018 11:43 am


## Using Docker with PHP 7


## Speed 2.5 secs to setup the everything I need 

# Make sure have intellij PHP Remote and Docker setup properly.
 

```bash


version: '2'
##https://github.com/JetBrains/phpstorm-docker-images/blob/master/docker-compose.yml
##PhpStorm Docker
services:
  webserver:
    image: phpstorm/php-71-apache-xdebug-26
    ports:
    - "80:80"
    volumes:
    - ./:/var/www/html
    environment:
      #change the line below with your IP address
      XDEBUG_CONFIG: remote_host=host.docker.internal

```
