FROM php:7.1.8-apache

MAINTAINER Adiputra

COPY . /var/www/html/laravel-docker
COPY .docker/vhost.conf /etc/apache2/sites-available/000-default.conf

RUN docker-php-ext-install mbstring pdo pdo_mysql \
&& chown -R www-data:www-data /var/www/html/laravel-docker \
&& a2enmod rewrite
