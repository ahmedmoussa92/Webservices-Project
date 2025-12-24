FROM php:8.1-apache

RUN apt-get update && apt-get install -y \
    libzip-dev zip unzip git curl \
    libpng-dev libonig-dev libxml2-dev \
    && docker-php-ext-install pdo_mysql zip intl gd

RUN a2enmod rewrite

WORKDIR /var/www/html
COPY src/ .

RUN chown -R www-data:www-data /var/www/html
