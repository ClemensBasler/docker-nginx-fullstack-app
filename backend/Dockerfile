FROM php:7.2-fpm-alpine

COPY ./www/html /var/www/html

#install git
RUN apk add --no-cache git

#install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# composer install
RUN composer install
