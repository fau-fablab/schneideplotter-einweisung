Schneideplotter Einweisung
==========================

Einweisung des [FAU FabLab](https://fablab.fau.de) in den [Schneideplotter](https://fablab.fau.de/tool/schneideplotter/) Roland CAMM-1 Servo GX-24.

Inhalt
------

- Regeln, erlaubte Materialien (Dicke, Größe, mit und ohne Trägerfolie)
- Material einlegen, Messer, Schnitttiefe, Offset, Anpressdruck und Geschwindigkeit einstellen
- Nullpunkt festlegen, Datei senden (CutStudio, Inkscape, Illustrator), Entgittern
- Verarbeitung: Aufkleber, T-Shirt-Folie, Etikettenpapier, Stiftplot

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/schneideplotter-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/schneideplotter-einweisung/Einweisung_Schneideplotter.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/schneideplotter-einweisung/Einweisungsliste_Schneideplotter.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/schneideplotter-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/schneideplotter-einweisung.git
cd schneideplotter-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/schneideplotter-einweisung/status.svg)](https://brain.fablab.fau.de/build/schneideplotter-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/schneideplotter-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/schneideplotter-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/schneideplotter-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/schneideplotter-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)

Ausnahme: Die Abbildungen von Roland sind nicht frei; solange es keinen Ersatz gibt, steht nur der Quelltext unter CC BY-SA 3.0.
