FROM php:apache
WORKDIR /var/www/html


RUN apt-get update \
  && apt-get install -y libfreetype6-dev libjpeg62-turbo-dev libpng12-dev libmcrypt-dev \
  && docker-php-ext-install pdo_mysql mysqli mbstring gd iconv mcrypt \

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer
