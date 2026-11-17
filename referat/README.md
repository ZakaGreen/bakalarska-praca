# Bakalársky projekt 1

В реферате разбираю SER и сравниваю его с MENTOR.

[PDF](../output/pdf/referat.pdf) · [LaTeX](../referat.tex) · [Библиография](bibliography.bib)

Сборка из корня репозитория (нужны LaTeX, latexmk и Biber):

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=referat/build referat.tex
```

Результат: `referat/build/referat.pdf`.
