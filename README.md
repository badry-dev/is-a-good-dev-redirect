# is-a-good-dev-redirect

GitHub Pages site that redirects **badry.is-a-good.dev** to **[https://badry.dev](https://badry.dev)**.

## Why

`is-a-good.dev` and `badry.dev` are both on Cloudflare. Pointing the subdomain CNAME directly at `badry.dev` triggers Cloudflare Error 1014 (CNAME Cross-User Banned). This repo hosts a static redirect on GitHub Pages instead; the is-a-good.dev register CNAME targets `badry-dev.github.io`.

## Files

- `index.html` / `404.html` — hard redirect (meta refresh + `location.replace`, path/query/hash preserved)
- `CNAME` — custom domain `badry.is-a-good.dev`
