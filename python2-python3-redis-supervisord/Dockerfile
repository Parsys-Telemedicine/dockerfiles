FROM ubuntu:xenial

# Install python3, pip (python2 version, for supervisor), redis-server then update pip and setuptools
RUN apt update \
 && apt upgrade -y \
 && apt install -y python python-pip python3 python3-pip python3-dev redis-server libpq5 vim \
 && rm -rf /var/lib/apt/lists/* \
 && pip2 -q --no-cache-dir install -U pip wheel setuptools \
 && pip -q install supervisor \
 && pip3 -q --no-cache-dir install -U pip wheel setuptools
