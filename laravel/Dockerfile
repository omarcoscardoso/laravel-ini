FROM php:8.0-cli AS builder

WORKDIR /var/www

RUN apt-get update && \
    apt-get install libzip-dev -y && \
    docker-php-ext-install zip

FROM php:8.0-fpm-alpine
WORKDIR /var/www
RUN chown -R www-data:www-data /var/www
EXPOSE 9000
CMD [ "php-fpm" ]