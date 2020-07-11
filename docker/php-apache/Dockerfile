
FROM php:7.2.1-apache


# Install Composer
ENV COMPOSER_ALLOW_SUPERUSER 1

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
    && composer --version

# Install ext php pdo mysql
RUN docker-php-ext-install pdo pdo_mysql mysqli