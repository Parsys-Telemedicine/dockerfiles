FROM node

RUN dpkg --add-architecture i386
RUN apt -qq update
RUN apt -qq upgrade -y
RUN apt -qq install -y nsis vim wine wine32
RUN rm -rf /var/lib/apt/lists/*
