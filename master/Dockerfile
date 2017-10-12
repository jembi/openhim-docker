FROM node:8

ENV NODE_ENV "production"

RUN node -v
RUN npm -v

WORKDIR /etc

# Update apt-repo list and install prerequisits
RUN apt-get update
RUN apt-get install -y git
RUN apt-get install -y bzip2

# Clone Openhim-console repo
RUN git clone https://github.com/jembi/openhim-core-js.git

WORKDIR /etc/openhim-core-js

# Install dependencies and build
RUN npm i
RUN npm run build

CMD ["node", "lib/server.js"]
