FROM centos:8

RUN dnf clean all
RUN dnf install -y https://rpms.remirepo.net/enterprise/remi-release-8.rpm

# PHPのインストール
RUN dnf install -y \
    php74 \
    php74-php-mcrypt \
    php74-php-mbstring \
    php74-php-fpm \
    php74-php-mysqlnd \
    php74-php-pdo \
    php74-php-xdebug

EXPOSE 9000

RUN \
    ln -s /usr/bin/php74 /usr/bin/php
