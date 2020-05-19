FROM golang:1.14.3-alpine3.11

RUN apk update && \
    apk add --no-cache ca-certificates git make && \
    GO111MODULE=off go get -u golang.org/x/tools/cmd/cover && \
    GO111MODULE=off go get -u github.com/t-yuki/gocover-cobertura

COPY codacy.sh .

ENTRYPOINT ["/bin/sh"]
