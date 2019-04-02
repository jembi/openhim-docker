FROM node:10.15.0

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

RUN curl -sL "https://github.com/jembi/openhim-core-js/archive/master.tar.gz" | \
    tar --strip-components=1 -zxvf - && \
    npm install && \
    npm run build && \
    npm cache clean --force

CMD ["node", "lib/server.js"]
