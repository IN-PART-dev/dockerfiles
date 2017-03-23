FROM node:7.4-alpine

# Install updates & dependencies
RUN echo "http://dl-cdn.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories \
 && apk update && apk upgrade \
 && apk add git python make g++ wget tar curl \
 && wget -P /tmp --quiet https://yarnpkg.com/latest.tar.gz; tar zxf /tmp/latest.tar.gz -C /tmp; rm /tmp/latest.tar.gz \
 && rm -rf /var/cache/apk/*

# Set path to yarn
ENV PATH /tmp/dist/bin:$PATH
