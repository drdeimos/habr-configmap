FROM golang:1.13-alpine

RUN apk update && apk add git
RUN go get github.com/fsnotify/fsnotify
RUN cd /go/src/github.com && git clone https://github.com/drdeimos/habr-configmap
RUN cd /go/src/github.com/habr-configmap/src && go build -o /bin/habr-configmap main.go
