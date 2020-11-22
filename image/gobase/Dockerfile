FROM golang:1.15-alpine

RUN apk update && \
    apk add --no-cache ca-certificates git make curl && \
    GO111MODULE=off go get -u -t github.com/volatiletech/sqlboiler && GO111MODULE=off go get github.com/volatiletech/sqlboiler/drivers/sqlboiler-psql && \
    GO111MODULE=off go get -u github.com/vektah/dataloaden && \
    GO111MODULE=off go get golang.org/x/tools/cmd/goimports && \
    curl -L https://github.com/vektra/mockery/releases/download/v2.3.0/mockery_2.3.0_Linux_x86_64.tar.gz | tar xzvf - && mv mockery /usr/bin/
