FROM ubuntu:bionic

# Install python3, pip, redis-server, weasyprint dependencies then update pip and setuptools.
RUN apt update \
 && apt upgrade -y \
 && apt install -y build-essential python3 python3-pip python3-dev python3-cffi libffi-dev redis-server libpq5 libcairo2 libpango1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 shared-mime-info vim \
 && rm -rf /var/lib/apt/lists/* \
 && pip3 -q --no-cache-dir install -U pip wheel setuptools \
 && hash -r pip \
 && pip3 -q install supervisor
