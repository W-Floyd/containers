# containers

Custom Caddy builds, published to `ghcr.io/<owner>/<name>:latest`.

| Image | Plugins |
| --- | --- |
| `caddy-umami` | [caddy-umami](https://github.com/jonaharagon/caddy-umami) |
| `caddy-cloudflare-umami` | [caddy-dns/cloudflare](https://github.com/caddy-dns/cloudflare), caddy-umami |

Base tags are pinned in each Dockerfile; Dependabot opens PRs to bump them.
Plugins build at their latest commit, picked up by the weekly rebuild.
