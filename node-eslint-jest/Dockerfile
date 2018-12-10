FROM node

RUN  apt -qq update \
 && apt -qq upgrade -y \
 && apt -qq install -y vim \
 && yarn global add eslint jest eslint-plugin-react babel-eslint eslint-config-standard-jsx eslint-config-standard eslint-plugin-import eslint-plugin-node eslint-plugin-promise eslint-plugin-standard eslint-plugin-jest\
 && rm -rf /var/lib/apt/lists/*
