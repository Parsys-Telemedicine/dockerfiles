FROM ubuntu:bionic

# Install python3, pip, weasyprint dependencies then update pip and setuptools.
RUN apt update
RUN apt upgrade -y
RUN apt install -y python3 python3-cffi python3-dev python3-pip build-essential iputils-ping libffi-dev libpq5 libcairo2 libpango1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 shared-mime-info vim
RUN rm -rf /var/lib/apt/lists/*
RUN pip3 install -q --no-cache-dir -U pip setuptools wheel
RUN hash -r pip
