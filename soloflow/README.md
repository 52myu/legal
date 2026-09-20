# SoloFlow legal pages

Hosted on GitHub Pages under:

**https://52myu.github.io/legal/soloflow/**

| Document | URL |
|----------|-----|
| Privacy Policy | https://52myu.github.io/legal/soloflow/privacy.html |
| Terms of Use (EULA) | https://52myu.github.io/legal/soloflow/terms.html |
| Support | https://52myu.github.io/legal/soloflow/support.html |

## Contents

- `privacy.html` — local-first data, OCR, subscriptions, analytics, **user-initiated exports**, **local notifications**, USD
- `terms.html` — EULA + Apple auto-renewal language + **not tax advice** + USD lock
- `support.html` — contact, FAQ (backup vs CPA, currency, reminders)

## App Store Connect

1. Publish these HTML files so they are reachable at `…/legal/soloflow/*.html` (must match live site after edits).
2. In App Store Connect set:
   - Privacy Policy URL → `https://52myu.github.io/legal/soloflow/privacy.html`
   - Support URL → `https://52myu.github.io/legal/soloflow/support.html`

App code reads the same URLs from `src/config/legalUrls.ts`.

**Important:** Editing files in this repo does not update GitHub Pages until you deploy/push the `legal` hosting repo (or whatever publishes `52myu.github.io`).
