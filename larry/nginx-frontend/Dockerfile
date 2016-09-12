FROM ubuntu:16.04
MAINTAINER Ili Vakalala "vakalik1@student.op.ac.nz"
ENV REFRESHED_AT 2014-06-01

RUN apt-get update
RUN apt-get -qqy install nginx

ADD nginx_proxy.conf /etc/nginx/nginx_proxy.conf

EXPOSE 80

CMD [ "nginx", "-g", "daemon off;" ]

