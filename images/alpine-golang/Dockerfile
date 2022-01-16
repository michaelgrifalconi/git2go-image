FROM golang:alpine
#TODO: use fixed version -> immutable builds

RUN apk update && apk add --no-cache bash git openssh alpine-sdk cmake openssl-dev python3

COPY images/setup-libgit2 /tmp/
RUN /tmp/setup-libgit2

WORKDIR /go/src/github.com/michaelgrifalconi/git2go-image
ENV GOBIN $GOPATH/bin

