# Zarafa
These settings can be set in /etc/zarafa/server.cfg and gateway.cfg.

## Medium security
```
server_ssl_protocols = !SSLv2 !SSLv3
server_ssl_ciphers = ALL:!LOW:!SSLv2:!SSLv3:!EXP:!aNULL
server_ssl_prefer_server_ciphers = yes or no
```

## High security
```
server_ssl_protocols = !SSLv2 !SSLv3 !TLSv1 !TLSv1.1  # >= Debian 7 / CentOS 7
server_ssl_ciphers = EECDH+ECDSA+AESGCM:EECDH+aRSA+AESGCM:EECDH+ECDSA+SHA384:EECDH+ECDSA+SHA256:EECDH+aRSA+SHA384:EECDH+aRSA+SHA256:EECDH+aRSA+RC4:EECDH:EDH+aRSA:RC4:!aNULL:!eNULL:!LOW:!3DES:!MD5:!EXP:!PSK:!SRP:!DSS
server_ssl_prefer_server_ciphers = yes or no
```
