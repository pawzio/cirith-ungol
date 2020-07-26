FROM golang:1.14.6-alpine3.12

RUN apk update && \
    apk add --no-cache ca-certificates git make curl && \
    GO111MODULE=off go get -u github.com/vektah/dataloaden && \
    curl -L https://github.com/vektra/mockery/releases/download/v2.1.0/mockery_2.1.0_Linux_x86_64.tar.gz | tar xzvf - && mv mockery /usr/bin/
