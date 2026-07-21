# GetDiscoverable.io

## Branding — read this first
- The name of this site is **GetDiscoverable.io** — always written with the "Get"
  prefix and the ".io". Never shorten it to "Discoverable" in copy, the nav/logo,
  the footer, meta tags, `llms.txt`, structured data, or anywhere else.
- Canonical domain: https://getdiscoverable.io
- Owner / author: Zillah Bahar, founder of COLAClear. COLAClear is used as the
  running worked example throughout the site.

## What this project is
A plain-English primer on SEO / AEO / GEO — how a business gets found by both
search engines and AI assistants. Static HTML/CSS, no build step, deployed on
Vercel with Vercel Web Analytics enabled.

## Analytics
- **Google Analytics 4** is the source of truth for campaign attribution.
  Measurement ID: **G-TZD5HHH2XE** (gtag.js is in the `<head>` of every page).
  Campaign numbers live under **Reports → Acquisition → Traffic acquisition →
  Session source / medium**.
- **Vercel Web Analytics** also runs (quick pageview glances only). Its free
  Hobby plan does NOT surface UTM parameters — that's why GA4 was added.

## UTM tagged-link kit
Rule: **one `utm_source` per channel, never reuse a link across channels.**
Base wine-post URL: `https://getdiscoverable.io/blog/why-ai-names-some-wineries/`

- **WIN:** `?utm_source=win&utm_medium=social&utm_campaign=wineries-post`
- **Punchdown:** `?utm_source=punchdown&utm_medium=social&utm_campaign=wineries-post`
- **LinkedIn:** `?utm_source=linkedin&utm_medium=social&utm_campaign=wineries-post`
- **COLAClear cross-links** (already live on colaclear.com): blog posts use
  `?utm_source=colaclear&utm_medium=blog&utm_campaign=winery-crosslink`; the
  Press page note uses `utm_medium=press`.

For a different post, keep the same `utm_source`/`utm_medium`/`utm_campaign`
convention and just change the base URL.
