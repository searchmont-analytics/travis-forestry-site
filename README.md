# travis-mccormack-forestry-analytics.com

Static portfolio site (HTML/CSS, one small script). No build step.

## Preview locally

    py -m http.server 8123 --directory site

## Deploy (GitHub Pages)

1. Push this folder's contents to a new repo, e.g. `searchmont-analytics/forestry-analytics-site`.
2. Settings → Pages → Deploy from branch `main`, folder `/ (root)`.
3. `CNAME` already holds the custom domain. At your registrar add DNS:
   - apex: A records 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `www`: CNAME → `searchmont-analytics.github.io`
4. Back in Settings → Pages, tick **Enforce HTTPS** once the certificate is issued.

## Before publishing

- Learning section: replace the "Public repo and live version coming soon" line (marked `TODO` in index.html)
  with the flashcard repo / live link once it's pushed.
- Optional: add a Cloudflare Web Analytics snippet (the analytics site uses one; this site has none yet).
