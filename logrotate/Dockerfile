FROM alpine:3.5

RUN apk add --no-cache logrotate

VOLUME ["/var/log"]

COPY ./rsyslog /etc/logrotate.d/rsyslog
RUN chmod 0644 /etc/logrotate.d/rsyslog

ENTRYPOINT ["crond", "-d", "6", "-f"]
