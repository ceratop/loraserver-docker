FROM ubuntu:16.04

WORKDIR /home/root

ENV LORA_APP_SERVER 0.6.0
ENV DOCKERIZE_VERSION v0.3.0

RUN apt-get update && apt-get install -y wget

RUN wget https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && tar -C /usr/local/bin -xzvf dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && rm dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz

ADD https://github.com/brocaar/lora-app-server/releases/download/${LORA_APP_SERVER}/lora_app_server_${LORA_APP_SERVER}_linux_amd64.tar.gz lora-app-server.tar.gz
ADD certs certs

RUN tar -xzf lora-app-server.tar.gz && rm -f lora-app-server.tar.gz

EXPOSE 8001

CMD ./lora-app-server

