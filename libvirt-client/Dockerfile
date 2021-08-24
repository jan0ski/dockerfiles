FROM alpine:latest
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apk --no-cache add \
	libvirt-client

ENTRYPOINT [ "virsh", "-c", "qemu:///system" ]
