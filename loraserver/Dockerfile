FROM ubuntu:16.04

WORKDIR /home/root

ENV LORASERVER_VERSION=0.15.1
ENV DOCKERIZE_VERSION v0.3.0

RUN apt-get update && apt-get install -y wget

RUN wget https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && tar -C /usr/local/bin -xzvf dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
    && rm dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz

ADD https://github.com/brocaar/loraserver/releases/download/${LORASERVER_VERSION}/loraserver_${LORASERVER_VERSION}_linux_amd64.tar.gz loraserver.tar.gz

RUN tar -xzf loraserver.tar.gz && rm -f loraserver.tar.gz

EXPOSE 8000

CMD ./loraserver
