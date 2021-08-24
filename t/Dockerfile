FROM	ruby:alpine
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN	apk add --no-cache \
	ca-certificates

RUN	set -x \
	&& apk add --no-cache --virtual .build-deps \
	build-base \
	&& gem install io-console t --no-document \
	&& apk del .build-deps

ENTRYPOINT	["t"]
