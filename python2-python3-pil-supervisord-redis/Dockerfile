FROM ubuntu:xenial

# Install python3, pip (python2 version, for supervisor), redis-server, PIL dependencies then update pip and setuptools
RUN apt update \
 && apt upgrade -y \
 && apt install -y python3 python3-pip python3-dev python3-lxml python3-cffi redis-server libpq5 libjpeg9 zlib1g libcairo2 libpango1.0-0 libgdk-pixbuf2.0-0 shared-mime-info \
 && rm -rf /var/lib/apt/lists/* \
 && pip3 -q --no-cache-dir install -U pip wheel setuptools \
 && pip2 -q --no-cache-dir install -U pip wheel setuptools \
 && pip2 -q install supervisor
