# InnerWave

Static site for [innerwave.health](https://innerwave.health), deployed as the Cloudflare Worker `innerwave`.

Pages:

- `/` — `public/index.html`
- `/science/` — `public/science/index.html`
- `/img/*` — `public/img/`

`wrangler.json` serves `public/` as Workers static assets. There is no compile step. `npm run build` only checks that those pages are present, then `npm run deploy` runs `wrangler deploy`.
