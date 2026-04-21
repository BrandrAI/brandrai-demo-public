# BrandrAI Public Demo Site

Public demo + marketing site deployed to `demo.brandrai.com` via Netlify.

## Structure

- `index.html` — redirect to landing page
- `02-landing-page-option-a.html` — main landing
- `03-coa-verify-page-with-blockchain-tease.html` — verify page (METRC-ANCHORED · LIVE PULL)
- `04/06/11/12/13/14-*.html` — vertical landings + team + pricing + bank + partner
- `17-20-*.html` — merchant/partner/bank dashboard mocks
- `18-coa-upload-flow.html` — interactive upload demo
- `26-pitch-deck-live.html` — interactive pitch deck
- `35-changelog-page.html` — public changelog (IP-safe)

## Excluded from this deploy

- Internal changelog (investors.brandrai.com — separate repo)
- Strategic markdown docs
- Word docs
- Python generation scripts

## Deploy

Netlify auto-deploys on every push to `main`.

To update from the Event Kit source folder:

```bash
cd "C:\Users\maxim\brandrai local test"
python publish_demo.py "your commit message"
```

That script:
1. Syncs `10 - May 1 Event Kit` → `BrandrAI DEMO WEB ONLY`
2. `git add` + `commit` + `push` with your message
3. Netlify deploys in ~30 seconds
