FROM node:6

# Install python3, pip (python2 version, for supervisor), redis-server, PIL dependencies then update pip and setuptools
RUN apt update \
 && apt upgrade -y \
 && apt install -y python3 python3-pip python-pip redis-server libpq5 libjpeg8 libtiff5 libxslt1.1 python-lxml libcairo2 libglib2.0 libffi6 libpango1.0-0 \
 && rm -rf /var/lib/apt/lists/* \
 && pip3 -q --no-cache-dir install -U pip wheel setuptools \
 && pip2 -q --no-cache-dir install -U pip wheel setuptools \
 && pip2 -q install supervisor
