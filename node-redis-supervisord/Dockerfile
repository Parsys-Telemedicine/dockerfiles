FROM node:10

# Install python3 and pip then update pip and setuptools.
RUN apt update
RUN apt upgrade -y
RUN apt install -y python3 python3-pip redis-server
RUN rm -rf /var/lib/apt/lists/*
RUN pip3 -q --no-cache-dir install -U pip wheel setuptools
RUN hash -r pip
RUN pip3 -q install supervisor
RUN npm i -g sequelize-cli pg
