FROM nginx:alpine

WORKDIR /usr/share/nginx/html

ENV OPENHIM_CONSOLE_VERSION 1.12.0

RUN wget "https://github.com/jembi/openhim-console/releases/download/v$OPENHIM_CONSOLE_VERSION/openhim-console-v$OPENHIM_CONSOLE_VERSION.tar.gz"

RUN tar xzf "openhim-console-v$OPENHIM_CONSOLE_VERSION.tar.gz"