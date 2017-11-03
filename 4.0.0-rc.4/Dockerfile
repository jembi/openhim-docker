FROM node:8.7.0

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ENV OPENHIM_CORE_VERSION 4.0.0-rc.4

RUN npm update npm -g

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/v$OPENHIM_CORE_VERSION.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    npm install && \
    npm run prepublish

CMD ["node", "lib/server.js"]
