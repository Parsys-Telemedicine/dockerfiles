FROM node

RUN apt -qq update \
 && apt -qq upgrade -y \
 && apt -qq install -y nsis wine \
 && rm -rf /var/lib/apt/lists/*
