FROM lyberteam/php-fpm-7.1

RUN docker-php-ext-install pcntl

RUN apt-get update

RUN apt-get install -y libxslt-dev

RUN apt-get install -y libicu-dev

RUN pecl install intl

RUN docker-php-ext-install intl

RUN docker-php-ext-install xsl

RUN docker-php-ext-install soap

RUN sed -i 's/memory_limit = 128M/memory_limit = 512M/g' /usr/local/etc/php/php.ini

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

CMD ["php-fpm"]