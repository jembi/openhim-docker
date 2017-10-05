FROM ubuntu:16.04

WORKDIR /etc/

RUN apt-get update
RUN apt-get install -y git
RUN apt-get install -y bzip2
RUN apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_8.x | bash -
RUN apt-get install -y nodejs
RUN git clone https://github.com/jembi/openhim-console.git

WORKDIR /etc/openhim-console

RUN npm i
RUN npm run build
RUN npm i -g http-server 
CMD http-server ./dist -p 80