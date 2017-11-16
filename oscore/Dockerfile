FROM alpine:latest
MAINTAINER Ali Sarchami "ali.sarchami@gmail.com"

RUN apk update && \
    apk upgrade && \
    apk add python2-dev py2-pip git gcc

RUN apk add musl-dev libffi-dev libressl-dev
RUN apk add libxml2-dev libxslt-dev
