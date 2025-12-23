FROM php:8.2-fpm

RUN apt-get update && apt-get install -y \
    libzip-dev unzip git curl libpng-dev libonig-dev libxml2-dev \
    libxslt1-dev libicu-dev \
    && docker-php-ext-install \
    pdo_mysql zip intl gd soap bcmath xsl

WORKDIR /var/www/html
