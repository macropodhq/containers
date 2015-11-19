FROM debian:jessie

RUN apt-get update \
 && apt-get install -y --force-yes --no-install-recommends\
      build-essential \
      curl \
      ca-certificates \
      git \
      lsb-release \
      python-all \
      rlwrap \
      imagemagick \
 && rm -rf /var/lib/apt/lists/*;

RUN curl https://deb.nodesource.com/node/pool/main/n/nodejs/nodejs_0.10.40-1nodesource1~jessie1_amd64.deb > node.deb \
 && dpkg -i node.deb \
 && rm node.deb \
 && npm install -g npm

