FROM node:8

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ENV OPENHIM_CORE_VERSION 4.0.0-rc.4

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/v$OPENHIM_CORE_VERSION.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    yarn install --pure-lockfile && \
    yarn cache clean && \
    yarn run build
    

CMD ["node", "lib/server.js"]
