FROM resin/raspberrypi2-alpine:latest

MAINTAINER Henry Seurer "henryse@gmail.com"

ARG PROJECT_VERSION=latest
ARG PROJECT_NAME=not_defined

RUN apk add --update curl && rm -rf /var/cache/apk/*
ADD entrypoint.sh /
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
CMD ["curl"]