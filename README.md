# Raporty Merry

Centralny hub raportów i materiałów zespołu marketingu north.pl (Ana, Kuba, Zosia, Marek, Tomek).
Wzorowany na strukturze `raporty-grzegorza` (agencja SEO/UX north.pl).

Publikowany jako statyczna strona — `index.html` w roocie repo można wystawić przez GitHub Pages
albo dowolny hosting statyczny (np. p4h.pl).

## Struktura

```
raporty-merry/
├── index.html              ← hub: lista projektów i linki do raportów
├── README.md                ← ten plik
├── szablony/
│   └── raport-szablon.html  ← szablon pojedynczego raportu, kopiuj dla nowego dokumentu
└── projekty/
    └── <nazwa-projektu>/
        ├── index.html        ← raport(y) HTML danego projektu
        └── pliki/             ← XLSX/CSV do pobrania (opcjonalnie)
```

## Jak dodać nowy raport

1. Jeśli to nowy projekt/kampania — stwórz folder `projekty/<nazwa-projektu>/`.
2. Skopiuj `szablony/raport-szablon.html` do tego folderu i wypełnij treścią.
3. W `index.html` (root) dodaj nowy blok `<div class="project">…</div>` (skopiuj istniejący blok
   „Przykładowa kampania" jako wzór) z linkiem do nowego raportu.
4. Numeruj dokumenty w kolejności priorytetu czytania: `01`, `02`, `03`…
   Oznaczenia: ⭐ KEY (kluczowy, czytać najpierw) · 🚀 DEV (gotowe do wdrożenia) ·
   📋 (lista/checklista) · ✅ (zamknięte/zweryfikowane) · 🆕 NOWY (świeżo dodane, opis do uzupełnienia).
5. Zaktualizuj datę „Ostatnia aktualizacja" w nagłówku `index.html`.
6. Commit + push.

## Usunięcie przykładu

Folder `projekty/_przyklad-kampania/` i odpowiadający mu blok w `index.html` to działający
przykład konwencji — usuń oba, gdy dodasz pierwszy prawdziwy projekt.
