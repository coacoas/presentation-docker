FROM ubuntu:14.04
MAINTAINER Bill Carlson <bill@coacoas.net>

RUN apt-get update -y
RUN apt-get install -y nginx
RUN update-rc.d -f nginx remove && \
    echo "\ndaemon off;" >> /etc/nginx/nginx.conf

EXPOSE 80
EXPOSE 443

CMD ["nginx"]
