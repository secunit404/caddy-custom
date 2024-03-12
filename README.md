# caddy-custom

Caddy with integrated support for Cloudflare DNS-01 ACME verification challenges.

**Please see the official [Caddy Docker Image](https://hub.docker.com/_/caddy) for more detailed deployment instructions.**

## Images

Includes images for regular and alpine versions of Caddy. Each are rebuilt every Monday morning at 0300 UTC from the `:latest` and `:alpine` tags respectively. Visit this repository on [Docker Hub](https://hub.docker.com/r/plaexmstr/caddy-custom) to pull images.

## Requirements
1. A Cloudflare account
2. All domains you want to use with Caddy MUST be on your Cloudflare account, for any domains not through Cloudflare you must fall back to another verification method using the `tls` block [here](https://caddyserver.com/docs/caddyfile/directives/tls).

## Instructions:

1. Caddy [here](https://hub.docker.com/_/caddy)
2. Caddy-cloudflare [here][https://github.com/caddy-dns/cloudflare]