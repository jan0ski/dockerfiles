FROM alpine:latest
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apk --no-cache add \
	--repository http://dl-cdn.alpinelinux.org/alpine/edge/testing/ \
	gnuplot

ENTRYPOINT ["gnuplot"]
