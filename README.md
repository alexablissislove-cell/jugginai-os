# jugginai-os

Deployment config for the JugginAI Cloudflare OS instance at https://os.jugginai.net.

This repo keeps only our `deployment.jsonc`. It does not vendor [cloudflare-os](https://github.com/cloudflare/cloudflare-os) or the official starter.

## Deploy

1. Clone [cloudflare/cloudflare-os-starter](https://github.com/cloudflare/cloudflare-os-starter).
2. Replace its `deployment.jsonc` with the file in this repo.
3. Follow the starter README to deploy (`pnpm install`, then the `cf-os` deploy flow).

Workers are named `jugginai-os-*`. The router custom domain is `os.jugginai.net`. Sign-in is Cloudflare Access; the admin email is in `deployment.jsonc`.
