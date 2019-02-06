FROM node:10.10.0

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ENV OPENHIM_CORE_VERSION 5.0.0

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/v$OPENHIM_CORE_VERSION.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    yarn install --pure-lockfile && \
    yarn cache clean && \
    yarn run build


CMD ["node", "lib/server.js"]
