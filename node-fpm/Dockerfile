FROM node

RUN apt -qq update \
 && apt -qq upgrade -y \
 && apt -qq install -y ruby-dev \
 && rm -rf /var/lib/apt/lists/* \
 && gem install fpm
