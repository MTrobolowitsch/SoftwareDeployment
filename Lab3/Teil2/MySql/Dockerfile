FROM debian:jessie

ENV DB_NAME=manueldb
ENV DB_USER=manuel
ENV DB_PASSWORD=qwert12345

USER root
RUN apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get install -y mysql-server
COPY docker-entrypoint.sh docker-entrypoint.sh
COPY install.sh install.sh
COPY init.sql /docker-entrypoint-initdb.d/
RUN ./install.sh
ENTRYPOINT ./docker-entrypoint.sh
EXPOSE 3306