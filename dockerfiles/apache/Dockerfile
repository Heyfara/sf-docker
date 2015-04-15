FROM tutum/apache-php

RUN apt-get update && apt-get -yq install php5-intl 

RUN a2enmod ssl
RUN a2enmod rewrite
RUN a2enmod suexec
RUN a2enmod include

RUN sed -i "s@^;date.timezone =.*@date.timezone = Europe/Paris@" /etc/php5/*/php.ini
