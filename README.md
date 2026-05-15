# [tbwtb.com](https://tbwtb.com)

They Became What They Beheld.

## Deploy

Deployed to the `tbwtb-com` Cloudflare Worker (Workers Static Assets) on push to `main` via `.github/workflows/deploy.yml`. The workflow runs `./build.sh` (substitutes commit hash and build time into `index.html`) then `wrangler deploy`. Worker config: `wrangler.jsonc`. Requires `CLOUDFLARE_API_TOKEN` repo secret.
