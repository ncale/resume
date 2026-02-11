# Resume

This repository contains the LaTeX source code for my resume.

## Formatting

I use [tex-fmt](https://github.com/WGUNDERWOOD/tex-fmt) for formatting the tex file.

```shell
tex-fmt resume.tex
```

## Automated Build

Every time a change is pushed to **master**, GitHub Actions automatically:

1. Compiles `resume.tex` using LaTeX.
2. Updates and pushes the latest `resume.pdf` directly to this repository.

The most up-to-date version is available here: [resume.pdf](https://ncale.github.io/resume/resume.pdf)
