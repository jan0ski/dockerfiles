FROM ubuntu:16.04
LABEL maintainer "jan0ski <mccormickt9@gmail.com>"

RUN apt-get update && apt-get install -y \
	software-properties-common \
	--no-install-recommends && \
	add-apt-repository ppa:hollywood/ppa && \
	apt-get update && \
	apt-get install -y \
	byobu \
	hollywood \
	locate \
	mlocate \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/* \
	&& updatedb

ENV HOME /home/user
RUN useradd --create-home --home-dir $HOME user \
	&& chown -R user:user $HOME

WORKDIR $HOME
USER user

CMD [ "hollywood" ]
