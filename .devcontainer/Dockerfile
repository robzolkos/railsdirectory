FROM ruby:3.2.2-slim-bullseye

ENV TZ="America/New_York"

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
  && apt-get -y install --no-install-recommends \
  apt-utils \
  build-essential \
  curl \
  git \
  imagemagick \
  iproute2 \
  openssh-client \
  default-libmysqlclient-dev\
  default-mysql-client\
  vim

RUN gem install bundler
RUN gem install foreman

WORKDIR /workspace
