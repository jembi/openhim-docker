FROM nginx:alpine

ENV OPENHIM_CONSOLE_VERSION 1.13.2

WORKDIR /etc
RUN wget -qO- "https://github.com/jembi/openhim-console/releases/download/v$OPENHIM_CONSOLE_VERSION/openhim-console-v$OPENHIM_CONSOLE_VERSION.tar.gz" | tar xvz

WORKDIR /usr/share/nginx
RUN rm -rf html
RUN ln -s /etc/openhim-console/dist html
