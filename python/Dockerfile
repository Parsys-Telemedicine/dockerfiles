FROM ubuntu:focal

# Install python3 and pip then update pip and setuptools.
RUN apt update
RUN apt upgrade -y
RUN apt install -y python3 python3-dev python3-pip iputils-ping language-pack-fr libpq5 vim
RUN rm -rf /var/lib/apt/lists/*
RUN pip3 install -q --no-cache-dir -U pip setuptools wheel
RUN hash -r pip
