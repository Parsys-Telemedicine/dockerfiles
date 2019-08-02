FROM ubuntu:bionic

# Install python3, pip, redis-server then update pip and setuptools.
RUN apt update \
 && apt upgrade -y \
 && apt install -y python3 python3-pip python3-dev redis-server libpq5 vim \
 && rm -rf /var/lib/apt/lists/* \
 && pip3 -q --no-cache-dir install -U pip wheel setuptools \
 && hash -r pip \
 && pip3 -q install supervisor
