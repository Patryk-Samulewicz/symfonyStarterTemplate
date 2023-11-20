FROM php:8.2-fpm-alpine

# Instalacja dodatków php.ini
RUN apk update && apk add --no-cache \
        libpq-dev \
    && docker-php-ext-install pdo pdo_pgsql

# Ustawienie katalogu roboczego
WORKDIR /var/www/symfony
