FROM php:7.2-apache

RUN apt update \
    && apt install nano \
    && docker-php-ext-install \
    pdo \
    pdo_mysql

COPY 000-default.conf /etc/apache2/sites-available
WORKDIR /var/www/html
