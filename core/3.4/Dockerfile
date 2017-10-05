FROM node:6

WORKDIR /etc

ENV OPENHIM_CORE_VERSION 3.4.0

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/v$OPENHIM_CORE_VERSION.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    npm install && \
    npm run prepublish

CMD ["node", "lib/server.js"]
