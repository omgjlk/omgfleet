FROM docker.io/debian:buster-slim

RUN apt-get update && apt-get install -y bip

COPY bip.conf /etc/bip/bip.conf
COPY bip.pem /etc/bip/bip.pem

EXPOSE 39393

CMD ["/usr/bin/bip", "-f", "/etc/bip/bip.conf", "-s", "/var/lib/bip", "-n"]
