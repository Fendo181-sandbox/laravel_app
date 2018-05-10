FROM php:7.2.5-fpm

# 作成したユーザの情報
MAINTAINER endu <fendo181git@gmail.com>

RUN apt-get update -y && apt-get install -y openssl zip unzip git
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
RUN docker-php-ext-install mbstring pdo_mysql

# serverを起動する。
WORKDIR /app
CMD php artisan serve --host=0.0.0.0 --port=8010
EXPOSE 8010
