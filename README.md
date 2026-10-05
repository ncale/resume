# Resume

This repository contains the LaTeX source code for my resume.

## Formatting

I use [tex-fmt](https://github.com/WGUNDERWOOD/tex-fmt) for formatting the tex file.

```shell
tex-fmt resume.tex
```

## Building

Use `pdflatex` for local builds.

```shell
pdflatex -output-directory=build resume.tex
```

## Automated Build

On every push, GitHub Actions compiles `resume.tex` using [latex-action](https://github.com/xu-cheng/latex-action), so a broken build fails on any branch.

On **main**, the compiled PDF is also deployed to Cloudflare Workers (static assets, configured in `wrangler.jsonc`). The latest version is always available at [resume.nickbrodeur.net](https://resume.nickbrodeur.net).

Deploying requires the `CLOUDFLARE_API_TOKEN` and `CLOUDFLARE_ACCOUNT_ID` repository secrets.
