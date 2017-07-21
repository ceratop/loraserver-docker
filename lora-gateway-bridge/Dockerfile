FROM ubuntu:16.04

WORKDIR /home/root

ENV LORA_GATEWAY_BRIDGE_VERSION 2.1.5

ADD https://github.com/brocaar/lora-gateway-bridge/releases/download/${LORA_GATEWAY_BRIDGE_VERSION}/lora_gateway_bridge_${LORA_GATEWAY_BRIDGE_VERSION}_linux_amd64.tar.gz .

#ADD https://github.com/brocaar/lora-gateway-bridge/releases/download/2.1.5/lora_gateway_bridge_2.1.5_linux_386.tar.gz lora_gateway_bridge.tar.gz

#RUN tar -xzf lora_gateway_bridge_${LORA_GATEWAY_BRIDGE_VERSION}_linux_amd64.tar.gz
#RUN rm -f lora_gateway_bridge_${LORA_GATEWAY_BRIDGE_VERSION}_linux_amd64.tar.gz

#RUN chmod +x lora-gateway-bridge

CMD ./lora-gateway-bridge
#CMD ls -lah 
