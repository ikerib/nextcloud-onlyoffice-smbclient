FROM nextcloud:fpm

RUN apt-get update && apt-get install -y procps smbclient && rm -rf /var/lib/apt/lists/*

RUN apt-get update && apt-get install -y smbclient libsmbclient-dev
RUN pecl install smbclient 
RUN docker-php-ext-enable smbclient
