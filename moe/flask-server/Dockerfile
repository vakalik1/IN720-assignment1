FROM python:2.7 
MAINTAINER Ili Vakalala "vakalik1@student.op.ac.nz"
ENV REFRESHED_AT 2016-08-01

ADD . /flask_server
WORKDIR /flask_server

RUN pip install -r requirements.txt
RUN uwsgi --build-plugin https://github.com/unbit/uwsgi-consul

ENTRYPOINT [ "uwsgi", "--ini", "uwsgi-consul.ini", "--ini", "uwsgi-consul.ini:server1" ]
CMD []
