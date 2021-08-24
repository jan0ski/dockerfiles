FROM alpine:latest
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apk add --no-cache \
	ca-certificates \
	py-boto


COPY ./reset-cache.py /bin/reset-cache.py

CMD [ "/usr/bin/python", "/bin/reset-cache.py" ]
