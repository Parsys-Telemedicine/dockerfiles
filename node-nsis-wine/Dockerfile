FROM node

RUN dpkg --add-architecture i386 \
 && apt -qq update \
 && apt -qq upgrade -y \
 && apt -qq install -y nsis vim wine wine32 \
 && wget -q -O /tmp/libpng12.deb http://mirrors.kernel.org/ubuntu/pool/main/libp/libpng/libpng12-0_1.2.54-1ubuntu1_amd64.deb \
 && dpkg -i /tmp/libpng12.deb \
 && rm /tmp/libpng12.deb \
 && rm -rf /var/lib/apt/lists/*
