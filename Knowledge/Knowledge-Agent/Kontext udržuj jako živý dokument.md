# Kontext udržuj jako živý dokument

## Trigger
- údržba agentické paměti
- neplatné odkazy v kontextu
- změny projektu nebo brandu

## Core rule
- Pokud agent narazí na starý kontext → oprav zdrojový dokument

## Decision rules
- Pokud agent použije starý odkaz nebo pravidlo → oprav kontextový dokument
- Pokud se změní brand, projekt nebo workflow → aktualizuj rozcestníky
- Pokud knowledge báze roste → spusť lint a zkontroluj zastaralost
- Živý kontext zvyšuje kvalitu budoucích odpovědí
- Neplatný kontext je horší než žádný kontext
- Údržba kontextu je opakovaný proces, ne setup na začátku projektu

## Use for
- údržbě AGENTS.md, CLAUDE.md nebo skillů
- aktualizaci brand manuálu
- přesunu zdrojů mezi nástroji
- kontrole knowledge báze po větší změně

## Avoid
- Brát kontextové soubory jako hotové jednou provždy a nechat agenta opakovat zastaralé instrukce

