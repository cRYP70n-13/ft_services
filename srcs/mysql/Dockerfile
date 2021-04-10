FROM alpine

# Basically this is not safe, so TODO: Change the user
USER root

COPY src/install.sh /tmp/install.sh
COPY src/start.sh /tmp/start.sh

RUN sh /tmp/install.sh

VOLUME [ "/var/lib/mysql" ]

EXPOSE 3306

ENTRYPOINT [ "sh", "start.sh" ]
