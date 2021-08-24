FROM golang:alpine as builder
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN	apk --no-cache add \
	ca-certificates \
	gcc \
	git \
	libc-dev

ENV PATH /go/bin:/usr/local/go/bin:$PATH
ENV GOPATH /go

RUN go get github.com/sourcegraph/checkup/cmd/checkup

FROM alpine:latest

COPY --from=builder /go/bin/checkup /usr/bin/checkup
COPY --from=builder /etc/ssl/certs/ /etc/ssl/certs

ENTRYPOINT [ "checkup" ]
