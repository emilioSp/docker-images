FROM php:5.6
RUN apt-get update && apt-get install -y zip
RUN pecl install xdebug-2.5.5
RUN docker-php-ext-install mysql pdo_mysql
RUN docker-php-ext-enable xdebug
RUN ln -snf /usr/share/zoneinfo/Europe/Rome /etc/localtime && echo 'Europe/Rome' > /etc/timezone
RUN echo '[PHP]\ndate.timezone = "Europe/Rome"\n' > /usr/local/etc/php/conf.d/tzone.ini