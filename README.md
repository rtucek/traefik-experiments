# Traefik experimens

...just tinkering around with [traefik's loadbalancer](https://traefik.io/).


## Setup

Only the self-signed certificates need to be generated.
For simplicity, I recommend using [mkcert](https://mkcert.dev/).

Simply run
```bash
mkcert \
	-cert-file ./certs/localhost-cert.pem \
	-key-file ./certs/localhost-key.pem localhost
docker-compose up
```


## Achievements

- [x] Support HTTP and HTTPS
- [x] Force redirect from HTTP to HTTPS
- [x] Make it work with self-signed certificate
- [x] Secure dashboard and API with TLS
