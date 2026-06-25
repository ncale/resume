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

Every time a change is pushed to **master**, GitHub Actions automatically:

1. Compiles `resume.tex` to pdf using [latex-action](https://github.com/xu-cheng/latex-action).
2. Commits and pushes the compiled result.

The latest version is always available here: [resume.pdf](https://ncale.github.io/resume/resume.pdf)
