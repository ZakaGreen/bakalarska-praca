[English](README.md) · [Slovenčina](README.sk.md) · [Русский](README.ru.md)

# Bakalárska práca — budúce udalosti a výnosy akcií

**Ilia Liubotin · aplikovaná informatika · FEI STU, Bratislava**

Téma výskumu: **predikcia vplyvu verejných správ a pravdepodobných budúcich udalostí na výnosy akcií pomocou jazykových modelov**.

## Súčasný stav

**Počiatočná fáza výskumu a prípravy.** Repozitár zatiaľ obsahuje prostredie na písanie v LaTeXu a materiály zo šablóny. Neobsahuje dokončenú prácu, natrénovaný predikčný model ani výsledky experimentov. Súbor `thesis.pdf` je pracovný dokument vychádzajúci zo šablóny.

## Smer výskumu

Skúmam, ako opísať udalosť, ktorá môže nastať v budúcnosti, a odhadnúť možnú reakciu akciového trhu, ak nastane.

Plánovaný prístup odlišuje dve otázky:

1. Aká je pravdepodobnosť, že udalosť nastane?
2. Aká reakcia môže nasledovať, ak nastane?

Historické správy a trhové dáta majú slúžiť na učenie a vyhodnocovanie. Hlavným záujmom je uplatniť tieto poznatky na **pravdepodobné budúce udalosti**, pričom treba zohľadniť časovú dostupnosť informácií a zabrániť úniku budúcich informácií (look-ahead bias). Ide o výskumné ciele, nie o hotové funkcie.

## Štruktúra repozitára

| Cesta | Účel |
| --- | --- |
| [thesis.tex](thesis.tex) | Hlavný dokument LaTeX a údaje o práci; niektoré polia zatiaľ obsahujú zástupné hodnoty. |
| [includes/](includes/) | Kapitoly, bibliografia a ďalšie textové materiály či súčasti šablóny. |
| [FEIstyle.cls](FEIstyle.cls) | Univerzitný štýl dokumentu bakalárskej práce. |
| [Makefile](Makefile) a [latexmkrc](latexmkrc) | Existujúca konfigurácia zostavenia LaTeXu. |

## Šablóna a zostavenie

Prostredie na písanie vychádza z [FEIStyle](https://github.com/Kyslik/FEIStyle). Pôvodná dokumentácia je zachovaná v [docs/FEIstyle-README.md](docs/FEIstyle-README.md) a pôvodná [licencia](LICENSE) zostáva na mieste.

S vhodnou distribúciou LaTeXu, nástrojmi `latexmk` a Biber a potrebnými balíkmi možno použiť existujúci Makefile:

```bash
make
```

Medzisúbory sa ukladajú do `.build/` a výsledný `thesis.pdf` do koreňa repozitára. Zostavenie práce nebolo pri aktualizácii dokumentácie portfólia znova spustené.
