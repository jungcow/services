FROM	alpine:3.12.0

RUN     apk update; apk add nginx; \
		apk add php7 \
                php7-fpm \
                php7-opcache \
                php7-gd \
                php7-mysqli \
                php7-zlib \
                php7-curl \
                php7-mbstring \
                php7-json \
                php7-session \
                php7-common \
                php7-session \
                php7-iconv \
                php7-xml \
                php7-imap \
                php7-cgi \
                fcgi \
                php7-pdo \
                php7-pdo_mysql \
                php7-soap \
                php7-xmlrpc \
                php7-posix \
                php7-mcrypt \
                php7-gettext \
                php7-ldap \
                php7-ctype \
                php7-dom

COPY	./srcs/init.sh ./
COPY	./srcs/config.inc.php ./
COPY	./srcs/nginx.conf ./

EXPOSE	5000

CMD		["sh", "init.sh"]
