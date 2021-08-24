# htop in a container
#
# docker run --rm -it \
# 	--pid host \
# 	jess/htop
#
FROM alpine:latest
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apk --no-cache add \
	htop

CMD [ "htop" ]
