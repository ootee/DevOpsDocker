FROM ubuntu:16.04

WORKDIR /mydir

RUN apt-get update && apt-get -y install curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN node -v && npm -v

CMD ["/bin/bash"]


# Ubuntu 16.04 with node.js
