FROM debian:sid-slim
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apt-get update && apt-get install -y \
	audacity \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT [ "audacity" ]
