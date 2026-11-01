# seo-score

SEO Score app for wedoart-il.com (GitHub Pages).

## Turn on the Rescan products button (one time)

On your computer, in a terminal:

1. `npm install -g @shopify/cli`
2. `git clone https://github.com/RonRdt/seo-score && cd seo-score`
3. `shopify app deploy` (sign in with the Shopify account that owns the app, confirm the release)
4. In Shopify admin open Apps > SEO Score and approve the new "read products" permission when asked.

Then click "Rescan products" on the SEO Score page.
