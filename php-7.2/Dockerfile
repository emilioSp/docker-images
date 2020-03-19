FROM php:7.2
RUN apt-get update
RUN apt-get install -y libicu-dev
RUN pecl install xdebug-2.6.0
RUN docker-php-ext-install pdo_mysql
RUN docker-php-ext-install intl
RUN docker-php-ext-enable xdebug
RUN ln -snf /usr/share/zoneinfo/Europe/Rome /etc/localtime && echo 'Europe/Rome' > /etc/timezone
RUN echo '[PHP]\ndate.timezone = "Europe/Rome"\n' > /usr/local/etc/php/conf.d/tzone.ini