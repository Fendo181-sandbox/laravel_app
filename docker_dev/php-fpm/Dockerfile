FROM php:7.2.5-fpm

# 作成したユーザの情報
MAINTAINER endu <fendo181git@gmail.com>

# install&update
RUN apt-get update && apt-get install -y \
		libmcrypt-dev \
		mysql-client \
    && pecl install mcrypt-1.0.1\
    && docker-php-ext-enable mcrypt
