# Kompletní raw zdroje bez zkracování

## Trigger
- ukládání transkriptů
- import primárních zdrojů
- pozdější reingesce

## Core rule
- Pokud ukládáš raw zdroj → ulož kompletní původní obsah bez zkrácení

## Decision rules
- Pokud ukládáš transkript → ověř, že je kompletní
- Pokud agent vytvoří raw soubor se zkrácenou částí → doplň plný text
- Pokud raw odkazuje na jiný nedostupný soubor → považuj zdroj za nekompletní
- Kompletní raw zdroj zvyšuje ověřitelnost znalostí
- Zkrácený raw zdroj snižuje schopnost pozdější reingesce
- Raw vrstva má uchovat fakta, ne interpretaci

## Use for
- YouTube transkriptech
- automatických titulcích
- přepisech schůzek
- importu webových článků

## Avoid
- Uložit do raw vrstvy jen shrnutí, výtah nebo poznámku „transkript zkrácen“

