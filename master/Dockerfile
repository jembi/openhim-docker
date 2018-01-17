FROM node:8

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/master.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    npm i

ENV NODE_ENV "production"

CMD ["node", "lib/server.js"]
