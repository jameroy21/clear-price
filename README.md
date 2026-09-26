# Clear Price v2.0.0

A stacked discount calculator. Type an original price and up to three stacked
discounts, and it shows the real final price live as you type. Discounts stack
sequentially: a 20% discount followed by a 70% discount is NOT 90% off.

Example: $89, 20% off, then 70% off -> you pay $21.36, you saved $67.64.

## What is new in v2

- Live calculation: the result updates as you type. No button to press.
- Cart: add multiple items, each with its own stacked discounts, plus one
  combined total that stays visible while you scroll.
- Currency switcher: USD ($), INR (₹), CAD (C$), TWD (NT$). Only the symbol
  changes; nothing is converted. Your phone's locale picks the starting
  currency, and you can override it.
- English and Spanish interface, switchable at the top of the app and
  remembered on your device.
- Discount fields appear as you use them, up to three per item.
- Your cart, currency, and language are saved on your device automatically.

## Install on your phone

This is a PWA (installable web app). It installs from its web address,
not from a downloaded file.

1. Host it: enable GitHub Pages on this repo (Settings -> Pages ->
   Deploy from a branch -> main, root). Your address becomes
   `https://<your-username>.github.io/clear-price/`.
2. Open that address on your phone.
3. Android (Chrome): three-dot menu -> Install app (or Add to Home screen).
4. iPhone (Safari): Share button -> Add to Home Screen.

The app then opens full screen like a native app and works offline.

## Owner view

The public app shows only the calculator plus a `© 2026 Jame Roy.
All rights reserved.` footer. The private owner view (SEO metadata,
share caption, copy buttons) opens by tapping the footer five times
quickly, or by opening the app with `?owner=1` in the address.

## Privacy

No login, no tracking, no analytics. Every calculation happens on the
device. Nothing leaves the phone.

## Files

- `index.html` — landing page and calculator (also the PWA entry)
- `assets/app.html` — installed-app entry the manifest points to
- `assets/manifest.webmanifest` — install metadata and icons
- `assets/service-worker.js` — offline caching
- `assets/icon-192.png`, `assets/icon-512.png`, `assets/apple-touch-icon.png`

© 2026 Jame Roy. All rights reserved.
