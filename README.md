# biome-docker

Small docker image for running Biome CLI.

## Usage

> You can specify the Architecture to use with `--build-arg ARCH=x64` or `--build-arg ARCH=arm64`.

```bash
cd dockerfiles && docker build -t biome-docker -f Dockerfile.alpine . # or Dockerfile.debian
docker run -it --rm --name biome-docker -v .:/data biome-docker check --apply .
```
