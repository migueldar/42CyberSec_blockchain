FROM debian

EXPOSE 80

RUN apt-get -y update
RUN apt-get -y install nginx

ENTRYPOINT nginx; tail -f /dev/null
