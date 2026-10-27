# learn.5at4am.me

A small standalone static page for the learn subdomain.

## Stack

Plain HTML and CSS. No build step, no JavaScript, no external fonts.

## Files

- `index.html`: the landing card and its metadata.
- `styles.css`: zinc design tokens, light and dark palettes, reduced-motion rules.
- `og.png`: 1200 by 630 social preview image.
- `manifest.webmanifest`: app name, theme, and install icons.
- `favicon.svg`, `favicon.ico`, `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`: icons.
- `404.html`: custom not-found page with `noindex`.
- `robots.txt` and `sitemap.xml`: crawl and discovery files.

## SEO

- Self-referencing canonical at `https://learn.5at4am.me/`
- Index and follow directives for search engines and Googlebot
- Open Graph and Twitter cards with a dedicated 1200 by 630 image
- JSON-LD for `WebSite`, `WebPage`, `BreadcrumbList`, and the publisher
- One canonical URL in the sitemap
- Custom 404 with `noindex`
- Manifest, PNG icons, and an SVG fallback, plus a theme color for mobile browsers

## Deploy

GitHub Pages serves the `main` branch from the repository root.

The `CNAME` file points the site at `learn.5at4am.me`.

## DNS

The `learn` CNAME should target `5at4am.github.io`. Pointing the subdomain at the apex `5at4am.me` can serve the page over HTTP, but GitHub Pages will not provision the TLS certificate for the subdomain.
