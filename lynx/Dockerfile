# Run Lynx in a conatiner
#
# docker run --rm -it \
#	--name lynx \
#	jess/lynx github.com/jessfraz
#
FROM debian:bullseye-slim
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apt-get update && apt-get install -y \
	lynx \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT [ "lynx" ]
