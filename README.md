# Gerry's Personal Home Page

Hugo site for Gerry's personal home page.

[Live Site](https://gshaw.ca)

## Build Instructions

```sh
brew install mise
mise install
mise run dev
```

`mise run dev` serves the site on `localhost:4001` with live reload and opens a browser.

Deploy with `mise run deploy`. It refuses unless you're on a clean `main` with nothing newer on GitHub, then checks, pushes, waits for Workers Builds and runs `mise run verify`. `mise run deploy-status` says whether `main` is live. The rule is in [Workshop's deploy note](https://github.com/gshaw/Workshop/blob/main/Tooling/deploy.md).

`mise run check` runs the build, spell check, Markdown lint and internal link check.

## Powered By

- Domain registrar: [Cloudflare Registrar](https://www.cloudflare.com/products/registrar/)
- DNS: [Cloudflare DNS](https://www.cloudflare.com/dns/)
- Hosting: [Cloudflare Workers](https://workers.cloudflare.com), static assets, built by Workers Builds
- Build System: [Hugo](https://gohugo.io)
- CSS: [Pico.css](https://picocss.com)
