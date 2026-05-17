# Sture Website (sture.io)

Single-page static marketing site for Sture, the mission-to-machine
platform built at Leva Nu Pty Ltd.

The site is intentionally minimal and serves as a credibility surface
for prospects and partners across AUKUS-aligned autonomous-systems
programs.

## Structure

```
.
├── index.html        # The entire site
├── hero.jpg          # Coastal-test-range hero photograph (1915 x 547)
├── sture-logo.svg    # White wordmark (used in header)
├── favicon.svg       # Sture mark used as browser favicon
└── README.md
```

No build step. No dependencies. No JavaScript.

## Local preview

Open `index.html` directly in a browser, or run any static server
from this directory:

```sh
python3 -m http.server 8081
# then open http://localhost:8081
```

## Deployment

Deployed via Cloudflare Pages, connected to this repo. Every push to
`main` triggers a new deploy.

**Cloudflare Pages build settings:**

- Build command: *(none)*
- Build output directory: `/`
- Production branch: `main`

Custom domain: `sture.io` (configured in the Cloudflare Pages
dashboard).

## Brand source files

The Affinity Designer sources for the wordmark, favicon, and hero
photo crop live in the main Forge monorepo under `brand/sture/`.
Only the rendered web assets are mirrored here.
