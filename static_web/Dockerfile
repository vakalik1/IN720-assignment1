FROM ubuntu:16.04
MAINTAINER Ili Vakalala "vakalik1@student.op.ac.nz"
ENV REFRESHED_AT 2016-09-05

RUN apt-get -qqy update
RUN apt-get -y install nginx

ADD kitten.jpg /www/data/
ADD nginx.conf /etc/nginx/nginx.conf

EXPOSE 80

CMD [ "nginx", "-g", "daemon off;" ]
