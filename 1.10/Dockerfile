FROM nginx

WORKDIR /usr/share/nginx/html

ENV OPENHIM_CONSOLE_VERSION 1.10.0

RUN apt-get update; apt-get install -y curl

RUN curl -sL "https://github.com/jembi/openhim-console/releases/download/v$OPENHIM_CONSOLE_VERSION/openhim-console-v$OPENHIM_CONSOLE_VERSION.tar.gz" | \
    tar --strip-components=1 -zxvf -
