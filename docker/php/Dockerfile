FROM php:apache
WORKDIR /var/www/html


RUN apt-get update \
  && apt-get install -y libfreetype6-dev libjpeg62-turbo-dev libpng12-dev libmcrypt-dev \
  && docker-php-ext-install pdo_mysql mysqli mbstring gd iconv mcrypt curl git \

RUN curl https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
