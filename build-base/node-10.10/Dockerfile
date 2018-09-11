FROM node:10.10-alpine

# Install updates & dependencies
RUN echo "http://dl-cdn.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories \
 && apk update && apk upgrade \
 && apk add \
      git \
      python \
      make \
      g++ \
      wget \
      tar \
      curl \
      gzip \
      jq \
      bash \
      rsync \
 && rm -rf /var/cache/apk/* \
 && yarn global add lerna@2.9
