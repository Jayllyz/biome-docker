FROM alpine:3.20

ARG BIOME_VERSION=1.7.3

RUN apk add --no-cache curl

WORKDIR /usr/local/bin
RUN curl -L "https://github.com/biomejs/biome/releases/download/cli%2Fv${BIOME_VERSION}/biome-linux-x64-musl" -o biome \
    && chmod +x biome

WORKDIR /data
ENTRYPOINT ["/usr/local/bin/biome"]
