FROM php:7.3-fpm-alpine

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories \
    && apk update \
    && apk --no-cache add autoconf gcc g++ make libffi-dev openssl-dev unixodbc-dev \
    && docker-php-ext-install pdo_mysql \
    && pecl install sqlsrv pdo_sqlsrv swoole redis \
    && docker-php-ext-enable sqlsrv pdo_sqlsrv swoole redis