FROM ubuntu
MAINTAINER Kimbro Staken

RUN apt-get update
RUN apt-get install -y software-properties-common python
RUN add-apt-repository ppa:chris-lea/node.js
RUN echo "deb http://us.archive.ubuntu.com/ubuntu/ precise universe" >> /etc/apt/sources.list
RUN apt-get install -y nodejs
RUN mkdir /var/www

ADD app.js /var/www/app.js

EXPOSE 8080

CMD ["/usr/bin/nodejs", "/var/www/app.js"]
