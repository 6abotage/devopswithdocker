FROM ubuntu:16.04

WORKDIR /mydir
RUN apt-get update && apt-get install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs
RUN git clone https://github.com/docker-hy/frontend-example-docker.git
WORKDIR /mydir/frontend-example-docker
EXPOSE 5000
RUN npm install
CMD npm start