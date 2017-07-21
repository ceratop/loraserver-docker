FROM ubuntu:16.04

WORKDIR /home/root

ENV LORA_GATEWAY_BRIDGE_VERSION 2.1.5

ADD https://github.com/brocaar/lora-gateway-bridge/releases/download/${LORA_GATEWAY_BRIDGE_VERSION}/lora_gateway_bridge_${LORA_GATEWAY_BRIDGE_VERSION}_linux_386.tar.gz lora_gateway_bridge.tar.gz

RUN tar -xzf lora_gateway_bridge.tar.gz && rm -f lora_gateway_bridge.tar.gz

#EXPOSE 8000

CMD ./lora-gateway-bridge
