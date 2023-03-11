FROM alpine:3.16

LABEL maintainer="NGINX Inception Docker by chillion"

RUN apk --update add nginx vim curl openssl && \
    rm -rf /var/cache/apk/* && \
    mkdir -p /etc/nginx/ssl && \
    mkdir -p /var/run/nginx && \
    mkdir -p /var/www/wordpress && \
    adduser -u 82 -D -S -G www-data www-data && \
    chown -R www-data:www-data /var/www/wordpress && \
    openssl req -x509 -nodes -out /etc/nginx/ssl/inception.crt -keyout /etc/nginx/ssl/inception.key -subj "/C=FR/ST=IDF/L=Paris/O=42/OU=42/CN=chillion.42.fr/UID=chillion"

COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 443

CMD ["nginx", "-g", "daemon off;"]
