FROM alpine:latest
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apk --no-cache add \
	ca-certificates \
	python \
	py2-pip \
	&& pip install httpie httpie-unixsocket

ENTRYPOINT [ "http" ]
