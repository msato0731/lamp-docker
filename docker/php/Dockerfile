FROM php:7.2-apache-stretch
MAINTAINER msato

RUN apt-get update \
    && apt-get install -y libpq-dev \
    && docker-php-ext-install pdo_mysql pdo_pgsql
    
COPY php.ini /usr/local/etc/php