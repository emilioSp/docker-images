FROM php:5.6
RUN pecl install xdebug-2.5.5
RUN docker-php-ext-install mysql pdo_mysql
RUN docker-php-ext-enable xdebug