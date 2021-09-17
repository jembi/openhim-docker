FROM node:14.17.0

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ENV OPENHIM_CORE_VERSION 7.0.2

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/v$OPENHIM_CORE_VERSION.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    npm install && \
    npm run build && \
    npm cache clean --force

CMD ["node", "lib/server.js"]
