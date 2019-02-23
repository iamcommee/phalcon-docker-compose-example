# Pull base image ref: https://hub.docker.com/r/mileschou/phalcon/
FROM mileschou/phalcon:7.1-apache

# Install pdo_mysql
RUN docker-php-ext-install pdo_mysql

# Enable mod rewrite
RUN a2enmod rewrite

# Install nano text-editor
RUN apt-get update && apt-get install nano


