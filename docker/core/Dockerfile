FROM node:5.3.0-wheezy

RUN apt-get update && apt-get -y upgrade && apt-get -y install git bash

RUN npm install -g gulp bower nodemon apidoc

VOLUME ["/app"]
WORKDIR /app
