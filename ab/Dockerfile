# ab (apache benchmark)
# in a container
#
# docker run --rm -it \
# 	jess/ab
#
FROM alpine:latest
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apk --no-cache add \
	apache2-ssl \
	apache2-utils \
	ca-certificates \
	htop

ENTRYPOINT [ "ab" ]
