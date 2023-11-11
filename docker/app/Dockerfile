# コンテナのベースとしてamazonlinux:2023を指定
FROM amazonlinux:2023

RUN dnf -y update

RUN dnf -y install unzip \
    wget

# php、モジュール関連インストール
RUN dnf -y install php less php-intl \
    php-cli php-json php-common php-devel php-fpm \
    php-gd php-mysqlnd php-mbstring php-pdo php-xml php-pgsql

# unix socket
RUN mkdir /var/run/php-fpm
VOLUME [ "/var/run/php-fpm" ]

# RUN echo 'short_open_tag = On' >> /etc/php.ini
# RUN echo 'date.timezone = Asia/Tokyo' >> /etc/php.ini
EXPOSE 9000

ENTRYPOINT /usr/sbin/php-fpm -F

# composerインストール
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer
RUN composer self-update

# nodeのインストール
RUN curl -fsSL https://rpm.nodesource.com/setup_18.x | bash -
RUN dnf -y install nodejs

# npmのアップデート
RUN npm install -g npm@10.2.3

# コンテナのディレクトリ指定
WORKDIR /var/www/html