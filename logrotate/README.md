# Logrotate Dockerfile

Cron daemon in a lightweight Alpine Linux image with logrotate utility. Unlike the default rsyslog logrotate configuration, this /etc/logrotate.d/rsyslog inludes a `copytruncate` directive in order to preclude the need to send a "-HUP" to the rsyslog container.
