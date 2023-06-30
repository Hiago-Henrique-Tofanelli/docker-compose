FROM php:8.1-apache
RUN apt update
ENV DEBIAN_FRONTEND noninteractive
RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli
RUN apt-get update && apt-get install -y libpq-dev && docker-php-ext-install pdo pdo_pgsql