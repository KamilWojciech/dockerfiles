FROM kamilwojciech/debian

MAINTAINER Kamil Wojciech "wojciech.kamil@gmail.com"

ADD files/apt/dotdeb.list /etc/apt/sources.list.d/dotdeb.list

RUN apt-get update && apt-get install -y --force-yes \
    php5 \
    php5-cli \
    php5-common \
    php5-curl \
    php5-gd \
    php5-mcrypt \
    php5-memcache \
    php5-mysql \
    php5-pgsql \
    php5-redis \
    php5-xsl \
    php5-imagick \
    php5-intl

ADD files/php5/common.ini /etc/php5/common/common.ini
ADD files/php5/cli.ini /etc/php5/cli/cli.ini
ADD files/php5/apache.ini /etc/php5/apache2/apache.ini

RUN apt-get update && apt-get install -y --force-yes \
    apache2 \
    libapache2-mod-php5

EXPOSE 80

