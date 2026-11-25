# Gerry's Personal Home Page

Hugo site for Gerry's personal home page.

[Live Site](https://gshaw.ca)

## Build Instructions

```sh
brew install mise
mise install
mise run dev
```

`mise run dev` serves the site at `https://gs.dev.gshaw.ca` (hugo on :4030) with live reload and opens a browser.

Changes land through a PR, squash-merged. Merging is the deploy: Workers Builds deploys every push to `main`. Then, on an up-to-date `main`, `mise run deploy` checks, waits for Workers Builds and runs `mise run verify`. It refuses if `main` has commits GitHub doesn't, and never pushes. `mise run deploy-status` says whether `main` is live. The rule is in [Workshop's deploy note](https://github.com/gshaw/Workshop/blob/main/Tooling/deploy.md).

`mise run check` runs the build, spell check, Markdown lint and internal link check.

## Powered By

- Domain registrar: [Cloudflare Registrar](https://www.cloudflare.com/products/registrar/)
- DNS: [Cloudflare DNS](https://www.cloudflare.com/dns/)
- Hosting: [Cloudflare Workers](https://workers.cloudflare.com), static assets, built by Workers Builds
- Build System: [Hugo](https://gohugo.io)
- CSS: [Pico.css](https://picocss.com)
