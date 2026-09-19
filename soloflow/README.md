# SoloFlow legal pages (GitHub Pages)

Static HTML for App Store compliance.

**Published base URL:**

```text
https://52myu.github.io/legal/
```

| Page | URL |
|------|-----|
| Privacy Policy | https://52myu.github.io/legal/privacy.html |
| Terms of Use (EULA) | https://52myu.github.io/legal/terms.html |
| Support | https://52myu.github.io/legal/support.html |

## Contents

- `privacy.html` — Privacy Policy (local-first, on-device OCR, analytics limits)
- `terms.html` — Terms of Use with **Apple auto-renewal** language and link to [Apple Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/)
- `support.html` — Support / FAQ (App Store Support URL)

## Deploy

1. Publish these HTML files to the GitHub Pages site for `52myu.github.io/legal/` (e.g. repo `legal` root, or Pages path `/legal`).
2. In **App Store Connect → App Information**:
   - Privacy Policy URL → `https://52myu.github.io/legal/privacy.html`
   - Support URL → `https://52myu.github.io/legal/support.html`
3. For subscriptions, the paywall / EULA link should point to `terms.html` (or Apple Standard EULA). Terms already incorporate Apple’s auto-renew rules and Standard EULA.

Source copies live in this repo under `docs/soloflow/` for version control; deploy the three HTML files to the Pages site above.

## App Store numeric ID

After the app is created in App Store Connect, replace placeholder `id0000000000` in the client (Share / Rate links) with the real Apple ID, e.g. `https://apps.apple.com/app/id1234567890`.

Set in code:

```ts
// src/config/legalUrls.ts
export const APP_STORE_ID = "1234567890";
```

## Contact

Privacy / support email used in these pages: `alan2012186186@gmail.com` (update if you use a different public address).
