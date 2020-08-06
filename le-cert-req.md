---
date: 2020-08-06
tags:
  - letsencrypt
  - nginx
---

# Generating letsencrypt certificates without stopping your webserver

## 1. Create a simple shell script like this

##### `cert-req.sh` 

```python
certbot -n --agree-tos -d $1 -m $2 certonly \
  --standalone --cert-name $1 --preferred-challenges http \
  --http-01-port 4080 --no-eff-email --keep-until-expiring \
  --rsa-key-size 4096
```

Here:

  - **`$1`:** domain that you want to issue the certificate for
  - **`$2`:** Your email address
  
This script when invoked as follows:

##### `./cert-req.sh example.com mail@example.com example.org`

requests a certificate with `example.com` as the CNs. It can be extended to ask for and add more CNs to the certificate.[^certbot]

## 2. nginx needs to have this config

##### `/etc/nginx/sites-enabled/plain`

```perl
server {
  listen 80;
  location ^~ /.well-known/acme-challenge/ {
    proxy_pass http://127.0.0.1:4080;
  }

  location / {
    rewrite ^ https://$http_host$request_uri? permanent;
  }
}
```

[^certbot]: Certbot user guide: <https://certbot.eff.org/docs/using.html>