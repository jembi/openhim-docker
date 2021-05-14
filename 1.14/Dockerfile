FROM nginx:alpine

WORKDIR /usr/share/nginx/html

ENV OPENHIM_CONSOLE_VERSION 1.14.2

RUN wget -qO- "https://github.com/jembi/openhim-console/releases/download/v$OPENHIM_CONSOLE_VERSION/build.openhim-console.v$OPENHIM_CONSOLE_VERSION.tar.gz" | tar xvz
