FROM php:5.6-apache

RUN apt-get update \
  && apt-get install -y nodejs npm less git \
  && npm cache clean \
  && npm install n -g \
  && n stable \
  && ln -sf /usr/local/bin/node /usr/bin/node \
  && apt-get purge -y nodejs npm
