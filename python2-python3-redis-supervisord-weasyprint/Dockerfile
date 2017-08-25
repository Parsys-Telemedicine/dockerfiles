FROM ubuntu:xenial

# Install python3, pip (python2 version, for supervisor), redis-server, weasyprint dependencies then update pip and setuptools
RUN apt update \
 && apt upgrade -y \
 && apt install -y python python-pip python3 python3-pip python3-dev python3-lxml python3-cffi redis-server libpq5 libcairo2 libpango1.0-0 libgdk-pixbuf2.0-0 shared-mime-info vim \
 && rm -rf /var/lib/apt/lists/* \
 && pip2 -q --no-cache-dir install -U pip wheel setuptools \
 && pip2 -q install supervisor \
 && pip3 -q --no-cache-dir install -U pip wheel setuptools
