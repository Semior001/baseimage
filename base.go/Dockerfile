FROM golang:1.13-alpine
LABEL maintainer="Semior <ura2178@gmail.com>"

ENV CGO_ENABLED=0

RUN apk add --no-cache --update git bash curl tzdata && \
    cp /usr/share/zoneinfo/Europe/Moscow /etc/localtime && \
    rm -rf /var/cache/apk/*

RUN go get github.com/derekparker/delve/cmd/dlv
