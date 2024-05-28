FROM alpine:3.20

ARG BIOME_VERSION=1.7.3

WORKDIR /usr/local/bin
RUN wget -O biome "https://github.com/biomejs/biome/releases/download/cli%2Fv${BIOME_VERSION}/biome-linux-x64-musl" && \
    chmod +x biome

WORKDIR /data
ENTRYPOINT ["/usr/local/bin/biome"]
