# seo-score

SEO Score app for wedoart-il.com (GitHub Pages).

## Turn on the Rescan products button (one time)

On your computer, in a terminal:

1. `npm install -g @shopify/cli`
2. `git clone https://github.com/RonRdt/seo-score && cd seo-score`
3. `shopify app deploy` (sign in with the Shopify account that owns the app, confirm the release)
4. In Shopify admin open Apps > SEO Score and approve the new "read products" permission when asked.

Then click "Rescan products" on the SEO Score page.

## What the page does (version 3, November 2026)

- **Needs attention**: every product, collection and article below 100 in one list, with the exact reason, Edit / View links and a per-item Rescan.
- **Saved scans**: scan details are kept in the browser (IndexedDB), so lists survive a reload. "Since the previous scan" shows what dropped, improved or is new.
- **Extra checks** (not part of the score): FAQs missing in the 7 other languages, and hair products missing the `collection:hair-care` tag.
- **Bulk fixes** change product text in the store. They sit in their own box and need a second click to confirm.
- `collection:` tags do not count toward the 5-10 tag total.
- Export: "Export to-fix list" and "Export everything" save a CSV with barcodes.
