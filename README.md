# supportaudit.co.uk

Static marketing site for **Support Audit** — independent resident support file audits for
supported exempt accommodation (SEA) and transitional supported housing in England.

Plain HTML, no build step. Everything in the repo root is served as-is.

## Deploy (Cloudflare Pages)

1. Workers & Pages → Create → Pages → Connect to Git → `Jamiemac9/supportaudit`.
2. Production branch: `main`.
3. Framework preset: **None**. Build command: *(leave empty)*. Build output directory: `/`.
4. Deploy, then add `supportaudit.co.uk` under Custom domains.
5. Point `seaaudit.com` at this project as a redirect, so the old domain resolves here.

Every push to `main` deploys to production; other branches get preview URLs.

## What is here

| Path | Purpose |
| --- | --- |
| `index.html` and page folders | The 8 pages, each with its own JSON-LD |
| `assets/` | CSS, JS, Schibsted Grotesk woff2, logo SVGs, share image |
| `robots.txt` | Search and AI answer engines allowed by name |
| `sitemap.xml` | All 8 URLs with `hreflang="en-GB"` |
| `llms.txt` / `llms-full.txt` | Plain-text for language models |
| `_headers` | Security headers and asset caching |
| `_redirects` | Short URLs and legacy paths |
| `e1aec...txt` | IndexNow key file |

## Brand

Trades as **Support Audit** at supportaudit.co.uk (settled 21 October 2026).

Bare **SEA** means *supported exempt accommodation*, the sector term. It is not the brand
and must never be find-and-replaced.

The mark is the four rating bands: Gold `#E8B84A`, Green `#43B581`, Amber `#F0954A`,
Red `#E35D5D`. `logo.svg` is for dark backgrounds, `logo-on-light.svg` for light.
Wordmark text is outlined, so it renders without the webfont.

## Addresses

- `contact@supportaudit.co.uk` — general
- `dpo@supportaudit.co.uk` — data protection, subject access, DPA
- `audit@supportaudit.co.uk` — resident file intake

## Before launch

- [ ] Replace `[ICO number]` on `/about/` with the real ICO registration number, or remove
      commitment 06 until registration is confirmed.
- [ ] Verify the domain in Google Search Console and submit `/sitemap.xml`.
- [ ] Verify in Bing Webmaster Tools (import from Search Console) and submit the same sitemap.
- [ ] Check the booking form posts somewhere real.
- [ ] Confirm "founder and director" is the right title if the company is not yet incorporated.
