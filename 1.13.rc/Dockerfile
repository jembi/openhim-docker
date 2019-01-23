FROM nginx:alpine

WORKDIR /usr/share/nginx/html

ENV OPENHIM_CONSOLE_VERSION 1.13.0-rc.1

RUN wget -qO- "https://github.com/jembi/openhim-console/releases/download/v$OPENHIM_CONSOLE_VERSION/openhim-console-v$OPENHIM_CONSOLE_VERSION.tar.gz" | tar xvz
