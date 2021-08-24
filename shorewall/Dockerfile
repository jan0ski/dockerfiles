# shorewall in a container
#
# docker run --rm -it \
# 	--net host \
# 	--cap-add NET_ADMIN \
#	--privileged \
# 	jess/shorewall
#
FROM alpine:latest
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apk --no-cache add \
	shorewall \
	&& touch /var/log/messages

COPY ./etc /etc/shorewall

ENTRYPOINT [ "/usr/sbin/shorewall" ]
