# Syed Sabbih Haider Shah — portfolio

Static source for [sabbih-shah.github.io](https://sabbih-shah.github.io/).

The site is deliberately dependency-free: semantic HTML, one stylesheet, and a single line of JavaScript. The downloadable résumé is generated from `cv/Sabbih_Shah_CV.tex`.

## Local preview

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Build the résumé

The PDF is built from the checked-in LaTeX source with Tectonic:

```bash
tectonic --outdir cv cv/Sabbih_Shah_CV.tex
```

Confirm that the result remains two pages and that its text can be extracted before publishing it.

## Publish

Create a public repository named `sabbih-shah.github.io`, push this directory to its `main` branch, and select **Deploy from a branch → main / root** under **Settings → Pages**.
