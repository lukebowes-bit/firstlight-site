# firstlight-site — the First Light support site

Plain HTML, no build step. Served by GitHub Pages at:

- https://lukebowes-bit.github.io/firstlight-site/          (landing)
- https://lukebowes-bit.github.io/firstlight-site/privacy/  ← App Store "Privacy Policy URL"
- https://lukebowes-bit.github.io/firstlight-site/support/  ← App Store "Support URL"

This repo is public so Pages can serve it for free; the app's source lives in
the private `firstlight` repo.

## Turn Pages on (one time)

Repo → **Settings** → **Pages** → Source: **Deploy from a branch** →
Branch: **main**, Folder: **/ (root)** → Save. First publish takes a minute or two.

## The support address

`first.light1234567@gmail.com`, shown on the privacy and support pages.

## Preview locally

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Keeping it honest

The privacy page claims the app makes no network requests, has no analytics and
no accounts. That was verified against the source on 2026-09-21 (no `URLSession`,
no CloudKit, no third-party SDKs). **If that ever changes, update the page in the
same commit** — an inaccurate privacy policy is a review rejection and a legal
problem, in that order.

Fonts are copies of `Marketing/fonts/` in the app repo so the pages match the
App Store screenshots.
