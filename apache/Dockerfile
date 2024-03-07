FROM debian:12

RUN apt-get update && apt-get install -y apache2 libapache2-mod-php
RUN ln -sf /dev/stdout /var/log/apache2/access.log 
RUN ln -sf /dev/stderr /var/log/apache2/error.log

EXPOSE 80
EXPOSE 443

ENTRYPOINT [ "apachectl", "-D", "FOREGROUND"]
