FROM php:7.3.6-fpm-alpine3.9

RUN apk add bash mysql-client mysql

RUN docker-php-ext-install pdo pdo_mysql

WORKDIR /var/www

COPY . .

EXPOSE 8000

ENTRYPOINT ["php", "artisan", "serve"]

CMD [ "--host=0.0.0.0" ]
