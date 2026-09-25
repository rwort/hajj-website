# Hajj Companion website

Static site for the Hajj Companion app: a landing page and the privacy
policy linked from the App Store and Google Play listings. No build step.

- `index.html` — landing page
- `privacy.html` — privacy policy (the store "Privacy Policy URL")
- `assets/styles.css` — tokens mirror the app's `lib/core/theme`
- `assets/icon.svg` — the app icon's mark (from the app's `tool/icons`)

## Before publishing

1. Replace the placeholder links on the two store buttons in `index.html`
   (`href="#"`) with the real App Store and Google Play URLs.
2. Make sure `support@hajcompanion.app` and `privacy@hajcompanion.app`
   exist, or change both addresses (they appear in `index.html` and
   `privacy.html`).
3. Confirm the legal entity name in `privacy.html` §1 ("operated by Hajj
   Companion") and the hosting provider wording in §6.
4. Update the "Last updated" date in `privacy.html` whenever the policy
   changes.

## Hosting

Any static host works. For GitHub Pages: Settings → Pages → deploy from
`main`, root. The privacy page is then at `https://<host>/privacy.html`.

## Preview locally

    python -m http.server 8000

then open http://localhost:8000.
