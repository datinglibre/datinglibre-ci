FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update  \
    && apt-get install --no-install-recommends -y \
    ca-certificates \
    apt-transport-https \
    php  \
    php-fpm  \
    php-json  \
    php-gd  \
    php-curl  \
    php-simplexml  \
    php-pgsql  \
    php-intl  \
    php-mbstring  \
    postgresql-client  \
    composer  \
    npm  \
    gnupg2  \
    git  \
    p7zip-full  \
    zip  \
    unzip  \
    curl  \
    wget  \
    && rm -rf /var/lib/apt/lists/*
RUN wget -O- https://dl.google.com/linux/linux_signing_key.pub | gpg --dearmor | tee /usr/share/keyrings/google-chrome.gpg
RUN echo deb [arch=amd64 signed-by=/usr/share/keyrings/google-chrome.gpg] http://dl.google.com/linux/chrome/deb/ stable main | tee /etc/apt/sources.list.d/google-chrome.list
RUN apt-get update  \
    && apt-get install --no-install-recommends -y google-chrome-stable
RUN curl -sS https://get.symfony.com/cli/installer | bash
RUN mv /root/.symfony/bin/symfony /usr/local/bin/symfony
