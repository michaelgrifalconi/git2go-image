FROM alpine:latest
#TODO: use fixed version -> immutable builds

RUN apk update && apk add --no-cache bash git openssh alpine-sdk cmake openssl-dev python

COPY images/setup-libgit2 /tmp/
RUN /tmp/setup-libgit2

