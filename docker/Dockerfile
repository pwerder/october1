FROM ubuntu:20.04

ENV timezone=America/Sao_Paulo

RUN apt-get update && \
    ln -snf /usr/share/zoneinfo/${timezone} /etc/localtime && echo ${timezone} > /etc/timezone && \
    apt -y install software-properties-common && \
    add-apt-repository ppa:ondrej/php -y && \
    apt-get update && \
    apt-get install -y php7.4 && \
    apt-get install -y php7.4-ctype && \
    apt-get install -y php7.4-curl && \
    apt-get install -y php7.4-xml && \
    apt-get install -y php7.4-fileinfo && \
    apt-get install -y php7.4-gd && \
    apt-get install -y php7.4-json && \
    apt-get install -y php7.4-mbstring && \
    apt-get install -y php7.4-mysql && \
    apt-get install -y php7.4-sqlite3 && \
    apt-get install -y php7.4-zip && \
    apt-get install -y git && \
    apt-get install -y nano && \
    php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && php composer-setup.php && rm composer-setup.php && mv composer.phar /usr/local/bin/composer && chmod a+x /usr/local/bin/composer

EXPOSE 80

WORKDIR /var/www/html

ENTRYPOINT /etc/init.d/apache2 start && /bin/bash

CMD ["true"]

