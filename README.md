[English](README.md) · [Slovenčina](README.sk.md) · [Русский](README.ru.md)

# Bachelor's Thesis — Future Events and Stock Returns

**Ilia Liubotin · Applied Informatics · FEI STU, Bratislava**

Research topic: **predicting the effect of public news and likely future events on stock returns using language models**.

## Current status

**Early research and preparation stage.** This repository currently contains the LaTeX writing setup and template material. It does not yet contain a completed thesis, a trained prediction model or experimental results. The existing `thesis.pdf` is a working/template document.

## Research direction

I am exploring how to describe an event that may happen in the future and estimate the possible stock-market reaction if it occurs.

The planned approach distinguishes two questions:

1. How likely is the event to occur?
2. What reaction might follow if that event occurs?

Historical news and market data are intended for learning and evaluation. The central interest is applying that knowledge to **likely future events**, with careful attention to information timing and avoiding look-ahead bias. These are research aims, not completed capabilities.

## Repository structure

| Path | Purpose |
| --- | --- |
| [thesis.tex](thesis.tex) | Main LaTeX document and thesis metadata; some fields are still placeholders. |
| [includes/](includes/) | Chapters, bibliography and other writing/template material. |
| [FEIstyle.cls](FEIstyle.cls) | University thesis document style. |
| [Makefile](Makefile) and [latexmkrc](latexmkrc) | Existing LaTeX build configuration. |

## Template and build notes

The writing setup is based on [FEIStyle](https://github.com/Kyslik/FEIStyle). Its original documentation is preserved in [docs/FEIstyle-README.md](docs/FEIstyle-README.md), and the original [license](LICENSE) remains in place.

With a suitable LaTeX distribution, `latexmk`, Biber and the required packages installed, the repository's Makefile provides:

```bash
make
```

This uses `.build/` for intermediate files and writes `thesis.pdf` in the repository root. The thesis build was not rerun as part of the portfolio documentation update.
