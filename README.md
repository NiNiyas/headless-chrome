# Supported Architectures

Pulling `niniyas/headless-shell:latest` should retrieve the correct image for your arch.

The architectures supported by this image are:

- x64
- arm64

Docker Hub: [hub.docker.com/r/niniyas/headless-shell](https://hub.docker.com/r/niniyas/headless-shell) \
GHCR: [ghcr.io/niniyas/headless-shell](https://ghcr.io/niniyas/headless-shell)

Based on [westy92/headless-chrome-alpine](https://github.com/westy92/headless-chrome-alpine).

## Sample docker-compose
```
version: '3.9'
services:
  headlesschrome:
    container_name: HeadlessShell
    image: niniyas/headless-shell:latest
    ports:
      - 9222:9222
```

## Build

```
git clone https://github.com/NiNiyas/headless-chrome.git
cd headless-chrome
docker build -t headless-shell .
```
