FROM ubuntu:focal

# libpangocairo-1.0-0 depends on tzdata.
ENV DEBIAN_FRONTEND=noninteractive

# Install python3, pip, weasyprint dependencies then update pip and setuptools.
RUN apt update
RUN apt upgrade -y
RUN apt install -y python3 python3-cffi python3-dev python3-pip build-essential iputils-ping language-pack-fr libffi-dev libpq5 libcairo2 libpango-1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 shared-mime-info vim
RUN rm -rf /var/lib/apt/lists/*
RUN pip3 install -q --no-cache-dir -U pip setuptools wheel
RUN hash -r pip
