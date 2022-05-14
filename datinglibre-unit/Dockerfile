FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update  \
    && apt-get install --no-install-recommends -y \
    composer \
    zip \
    unzip \
    p7zip-full  \
    curl \
    wget \
    php  \
    php-fpm  \
    php-json  \
    php-gd  \
    php-curl  \
    php-simplexml  \
    php-pgsql  \
    php-intl  \
    php-mbstring \
    git \
    && rm -rf /var/lib/apt/lists/*