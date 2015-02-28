FROM kamilwojciech/apache-php55

MAINTAINER Kamil Wojciech "wojciech.kamil@gmail.com"

ADD files/apache/000-default.conf /etc/apache2/sites-enabled/000-default.conf

ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data

CMD ["/usr/sbin/apache2", "-d", "/etc/apache2", "-k", "start"]

