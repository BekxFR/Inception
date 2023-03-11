FROM debian:buster

LABEL maintainer="MARIADB Inception Docker by chillion"

RUN apt-get update \
    && apt-get install -y vim mariadb-server \
    && mkdir -p /var/run/mariadb

COPY 50-server.cnf	/etc/mysql/mariadb.conf.d/50-server.cnf
COPY mariadb-DBCreate.sh	/var/run/mariadb/mariadb-DBCreate.sh

EXPOSE 3306

ENTRYPOINT ["bash", "/var/run/mariadb/mariadb-DBCreate.sh"]
