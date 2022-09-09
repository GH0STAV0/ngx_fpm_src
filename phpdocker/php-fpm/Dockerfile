FROM phpdockerio/php:7.4-fpm
RUN pwd
RUN ls

ADD testp  /application

WORKDIR "/application"

RUN apt-get update; \
    apt-get -y --no-install-recommends install \
        php7.4-imap; \
    apt-get clean; \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*
 
