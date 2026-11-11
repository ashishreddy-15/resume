# Resume - Ashish Reddy Ette

[![Compile Resume PDF](https://github.com/ashishreddy-15/resume/actions/workflows/compile.yml/badge.svg)](https://github.com/ashishreddy-15/resume/actions/workflows/compile.yml)

This repository contains the LaTeX source code and automated build pipeline for my professional resume.

- **Source:** [`resume.tex`](resume.tex)
- **Compiled PDF:** [`resume.pdf`](resume.pdf)

## Automated CI/CD

Whenever changes are made to `resume.tex` and pushed to `main`:
1. GitHub Actions automatically compiles `resume.tex` using XeLaTeX and the bundled Inter font family.
2. The compiled `resume.pdf` is uploaded as an action artifact.
3. The latest `resume.pdf` is automatically committed and pushed back to the repository.

## Local Compilation

To compile locally using XeLaTeX:

```bash
xelatex resume.tex
```

Prerequisites:
- TeX Live with XeLaTeX (`texlive-xetex`)
- [Inter](https://rsms.me/inter/) font family (available in `fonts/`)
