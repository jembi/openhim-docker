FROM node:8

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/staging.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    yarn install --pure-lockfile && \
    yarn cache clean && \
    yarn run build

ENV NODE_ENV "production"

CMD ["node", "lib/server.js"]
