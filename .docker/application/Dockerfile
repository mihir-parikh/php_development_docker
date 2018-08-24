FROM php:7-apache

RUN apt-get update -y
RUN apt-get install -y curl libcurl4-openssl-dev
# Install other extensions as needed
RUN docker-php-ext-install pdo pdo_mysql mysqli curl

RUN a2enmod rewrite
RUN service apache2 restart

EXPOSE 80
