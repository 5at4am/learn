# learn.5at4am.me

A small standalone static page for the learn subdomain.

## Stack

Plain HTML and CSS. No build step, no JavaScript, no external fonts.

## Deploy

GitHub Pages serves the `main` branch from the repository root.

The `CNAME` file points the site at `learn.5at4am.me`.

## DNS

The `learn` CNAME should target `5at4am.github.io`. Pointing the subdomain at the apex `5at4am.me` can serve the page over HTTP, but GitHub Pages will not provision the TLS certificate for the subdomain.
