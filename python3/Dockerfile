FROM anyfiddle/ubuntu

USER root

RUN apt-get update && apt-get install -y \
	python3 \
	python3-pip \
	&& rm -rf /var/lib/apt/lists/*

RUN ln -s /usr/bin/python3 /usr/bin/python & \
    ln -s /usr/bin/pip3 /usr/bin/pip

USER anyfiddle

COPY --chown=anyfiddle ./workspace /home/anyfiddle/project