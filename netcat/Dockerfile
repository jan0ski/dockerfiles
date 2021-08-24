FROM debian:sid-slim
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apt-get update && apt-get install -y \
	netcat \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT [ "netcat" ]
