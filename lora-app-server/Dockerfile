FROM ubuntu:16.04

WORKDIR /home/root

ENV LORA_APP_SERVER 0.10.1

ADD https://github.com/brocaar/lora-app-server/releases/download/${LORA_APP_SERVER}/lora_app_server_${LORA_APP_SERVER}_linux_amd64.tar.gz lora-app-server.tar.gz

#RUN tar -xzf lora-app-server.tar.gz && rm -f lora-app-server.tar.gz

EXPOSE 8080
EXPOSE 8001

CMD ./lora-app-server

