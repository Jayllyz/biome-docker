ARG BIOME_VERSION=1.7.3
FROM alpine:3.20

WORKDIR /app

RUN wget -O biome "https://github.com/biomejs/biome/releases/download/cli%2Fv${BIOME_VERSION}/biome-linux-x64" \
    && chmod +x biome \
    && mv biome /usr/local/bin/biome

ENTRYPOINT ["biome"]
CMD ["--help"]
