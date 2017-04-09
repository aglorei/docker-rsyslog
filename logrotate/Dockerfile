FROM alpine:3.5

RUN apk add --no-cache logrotate

VOLUME ["/var/log", "/etc/logrotate.d"]

COPY ./rsyslog /etc/logrotate.d/rsyslog

ENTRYPOINT ["crond", "-d", "6", "-f"]
