# Rsyslog and Logrotate

This repository configures a host into a central syslog server with logrotate utility.

- [Rsyslog](https://github.com/robbert229/docker-rsyslog)
  - Binds external port 514 over TCP and UDP for remote syslog reachability
  - Writes to /var/log/syslog in shared volume `docker-rsyslog-storage`
- [Logrotate](logrotate/README.md)
  - Rotates /var/log/syslog in shared volume `docker-rsyslog-storage` daily

#### Quick Start:

```
docker-compose up -d
```

