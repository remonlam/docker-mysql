FROM remonlam/docker-mysql
MAINTAINER Remon Lam <remon.lam@virtualclouds.info>

ENV MYSQL_USER mysql
ENV TERM=xterm

COPY ./osx-start-db.sh /
RUN chmod 755 /osx-start-db.sh

ENTRYPOINT ["/osx-start-db.sh"]
