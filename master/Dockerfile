FROM node:8

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

# Update to the latest npm to work around https://github.com/npm/npm/issues/18520
RUN npm install -g npm

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/master.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    npm install && \
    npm cache clean --force && \
    npm run build

ENV NODE_ENV "production"

CMD ["node", "lib/server.js"]
