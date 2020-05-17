FROM golang:1.14.3-alpine3.11

RUN apk update && \
    apk add --no-cache ca-certificates git make && \
    GO111MODULE=off go get -u github.com/kyoh86/richgo
