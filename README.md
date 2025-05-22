# caddy-custom

[![Build Status](https://github.com/secunit404/caddy-custom/actions/workflows/build.caddy-custom.yml/badge.svg)](https://github.com/secunit404/caddy-custom/actions)
[![Docker Image](https://img.shields.io/badge/docker-ghcr.io%2Fsecunit404%2Fcaddy--custom-blue)](https://github.com/users/secunit404/packages/container/package/caddy-custom)

## Overview

This repository provides a Docker image of [Caddy](https://caddyserver.com/) with custom modules for advanced functionality. It is ideal for users who require DNS providers or other plugins not included in the official image.

## Included Modules

The current build includes the following modules:
- [Cloudflare DNS](https://github.com/caddy-dns/cloudflare)

*(This list is also reflected dynamically in image metadata and releases.)*

## Usage

### Pull image from GHCR

```bash
docker pull ghcr.io/secunit404/caddy-custom:latest
```

### Example: Running the container

```bash
docker run -d -p 80:80 -p 443:443 \
  -v $PWD/Caddyfile:/etc/caddy/Caddyfile \
  ghcr.io/secunit404/caddy-custom:latest
```

### Building locally

```bash
docker build -t my-caddy-custom ./caddy-custom
```

## Updating

Whenever a new Caddy version or module update is available, a new release is published automatically via GitHub Actions.

## More Information

- [Official Caddy Docker Instructions](https://hub.docker.com/_/caddy)
- [Latest Releases](https://github.com/secunit404/caddy-custom/releases)
- [Container Registry (GHCR)](https://github.com/users/secunit404/packages/container/package/caddy-custom)

## Contributing

PRs and suggestions are welcome!
