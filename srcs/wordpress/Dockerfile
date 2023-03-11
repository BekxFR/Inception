FROM debian:buster

LABEL maintainer="WORDPRESS Inception Docker by chillion"

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install vim wget -y && \
    apt-get install -y php7.3 php-fpm php-mysql mariadb-client && \
    wget -qO /tmp/wp-cli.phar https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar && \
    chmod +x /tmp/wp-cli.phar && \
    mv /tmp/wp-cli.phar /usr/local/bin/wp && \
    rm -rf /var/lib/apt/lists/* && \
    mkdir /var/www && cd /var/www && \
    wget -qO- https://fr.wordpress.org/latest-fr_FR.tar.gz -P /var/www | tar xvz && \
    chown -R root:root /var/www/wordpress

COPY www.conf	/etc/php/7.3/fpm/pool.d/www.conf

COPY WP-StartConfig.sh	/var/run/wordpress/WP-StartConfig.sh

EXPOSE 9000

ENTRYPOINT ["/var/run/wordpress/WP-StartConfig.sh"]
