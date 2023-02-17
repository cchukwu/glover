FROM php:8.0-fpm
RUN apt-get update -y && apt-get install -y openssl zip unzip git
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
#RUN docker-php-ext-install pdo mbstring

ENV COMPOSER_ALLOW_SUPERUSER=1
RUN apt-get install -y libonig-dev && docker-php-ext-install iconv mbstring

WORKDIR /app
COPY . /app
RUN composer update

CMD php artisan serve --host=0.0.0.0 --port=8080
EXPOSE 8080