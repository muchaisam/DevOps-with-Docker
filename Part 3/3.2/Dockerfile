FROM node:alpine

WORKDIR /app

RUN apt-get update

RUN apt-get install -y git

RUN git clone https://github.com/muchaisam/DarkLightToggle

RUN docker build -t muchaisam/DarkLightToggle