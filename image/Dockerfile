FROM resin/raspberrypi2-alpine:latest

MAINTAINER Henry Seurer "henryse@gmail.com"

ARG PROJECT_VERSION=latest
ARG PROJECT_NAME=not_defined

RUN apk add --update curl && rm -rf /var/cache/apk/*
COPY entrypoint.sh /
ENTRYPOINT ["/entrypoint.sh"]
CMD ["curl"]