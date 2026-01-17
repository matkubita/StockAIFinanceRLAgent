# Instrukcja Kompilacji Dokumentacji

W tym folderze znajduje się przykładowy raport LaTeX (`raport_a2c.tex`), który dołącza opis algorytmu A2C z pliku `../opis_a2c/opis_a2c.tex`.

## Wymagania
Aby skompilować dokument, musisz mieć zainstalowany system TeX/LaTeX. W systemie Linux (np. Ubuntu/Debian) najczęściej jest to pakiet `texlive`.

Instalacja podstawowa:
```bash
sudo apt-get install texlive-latex-base texlive-fonts-recommended texlive-fonts-extra texlive-lang-polish
```

## Kompilacja
Aby wygenerować plik PDF, uruchom w terminalu, będąc w tym folderze:

```bash
pdflatex raport_a2c.tex
```

Polecenie to utworzy plik `raport_a2c.pdf`. Czasami wymagane jest dwukrotne uruchomienie kompilacji, aby poprawnie wygenerować spisy treści lub odnośniki (jeśli są używane).

## Czyszczenie (Clean)
Po kompilacji powstaje wiele plików pomocniczych (`.aux`, `.log`, `.fls`, `.fdb_latexmk` itp.). Aby je usunąć i zostawić tylko plik PDF oraz źródła, możesz użyć polecenia:

```bash
rm -f *.aux *.log *.out *.toc *.fls *.fdb_latexmk *.synctex.gz
```

Lub jeśli masz zainstalowane narzędzie `latexmk`:
```bash
latexmk -c
```
