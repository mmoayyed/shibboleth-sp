## Overview

This Docker image is Apache 2.4 with Shibboleth SP 3 installed running on CentOS.

Ports 80 and 443 are exposed for traffic.

## Logs

Logs for httpd and shibd have been configured to output to the console so that Docker's logging facilities are supported. Each of these logs have been prefaced with an identifier that indicates the type of entry being outputted: `httpd-error`, `httpd-combined`, `sp-shibd`, `sp-native`, `sp-transaction`, `sp-sign`, etc.

```
docker build --tag="mmoayyed/shibboleth-sp" .
```
