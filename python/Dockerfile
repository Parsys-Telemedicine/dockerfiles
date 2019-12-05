FROM ubuntu:bionic

# Install python3 and pip then update pip and setuptools.
RUN apt update
RUN apt upgrade -y
RUN apt install -y python3 python3-pip python3-dev libpq5 vim
RUN rm -rf /var/lib/apt/lists/*
RUN pip3 -q --no-cache-dir install -U pip wheel setuptools
RUN hash -r pip
