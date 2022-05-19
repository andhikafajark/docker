# FROM php:fpm-alpine
FROM php:fpm

RUN apt-get update && apt-get install -y --no-install-recommends libpq-dev \
    && docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
    && docker-php-ext-install mysqli pgsql pdo pdo_mysql pdo_pgsql