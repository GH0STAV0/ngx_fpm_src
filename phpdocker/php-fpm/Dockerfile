FROM phpdockerio/php:7.4-fpm
RUN pwd
RUN ls



WORKDIR "/application"
ADD ./phpdocker/php-fpm/  /application/
RUN ls /application/*
RUN apt-get update; \
    apt-get -y --no-install-recommends install \
        php7.4-imap; \
    apt-get clean; \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*
    
 EXPOSE 8080
 
