# chartingdecoded.com

One-page site for **The Evidence-Based Trading Series** by Nathan Calderay.

## Deploy (Vercel)
Static — no build step. Drag this folder into Vercel, or:

    vercel --prod

Then point `chartingdecoded.com` at the project in Vercel's domain settings.

## Structure
    index.html            entire site
    assets/covers/*.jpg   book covers (800x1200, optimised)
    vercel.json           clean URLs + cache headers for assets

## Design notes
Palette and type are lifted from the covers: spine navy `#101B2D`, cover stock
`#F3EFE8`, gold `#B0812A`, Elliott blue `#3F6088`, Wyckoff green `#16341F`.
Oswald (condensed titles) / Barlow (body) / Cormorant Garamond (author name),
matching the cover hierarchy.

The **left spine rail** is the signature device — it reproduces the physical book
spine, and tracks which book you're scrolled to (number + accent colour).
It hides below 860px.

## Before launch — TODO
1. **Check the affiliate links** resolve to the right books.
2. **Set the contact email** — `hello@chartingdecoded.com` is a placeholder.
3. Optional: add `og-image.jpg` (1200x630) and reference it in the `og:image` meta.

No forms, no backend, no data collected — the only outbound paths are the four
Amazon links.

## Adding the indicators later
The `#tools` section is built to become a storefront: replace the
`<p class="tools-status">` + button with buy links (Payhip/Stripe), drop the
`In progress` badge, and the mock chart panel stays as the product visual.
