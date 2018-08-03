FROM ubuntu:16.04
MAINTAINER rdp89 rafadelgado89@gmail.com

RUN apt-get update
RUN apt-get -y install nginx
ADD nginx.html /var/www/html
RUN mkdir /var/www/html/docker
ADD index.html /var/www/html/docker
ADD default /etc/nginx/sites-enabled/default
RUN chown -R www-data:www-data /var/www/html
CMD nginx -g 'daemon off;'
