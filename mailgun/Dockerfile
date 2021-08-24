FROM r.j3ss.co/curl
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apk add --no-cache \
	bash

COPY sendemail /usr/bin/sendemail

ENTRYPOINT [ "sendemail" ]
