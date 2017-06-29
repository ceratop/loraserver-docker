FROM ubuntu:16.04

WORKDIR /home/root

ENV LORASERVER_VERSION 0.19.1

ADD https://github.com/brocaar/loraserver/releases/download/${LORASERVER_VERSION}/loraserver_${LORASERVER_VERSION}_linux_amd64.tar.gz loraserver.tar.gz

RUN tar -xzf loraserver.tar.gz && rm -f loraserver.tar.gz

EXPOSE 8000

CMD ./loraserver
