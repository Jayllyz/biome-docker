# biome-docker

Small docker image for running Biome CLI.

## Usage

```bash
cd dockerfiles && docker build -t biome-docker -f Dockerfile.alpine . # or Dockerfile.debian
docker run -it --rm --name biome-docker -v .:/data biome-docker check --fix
```
