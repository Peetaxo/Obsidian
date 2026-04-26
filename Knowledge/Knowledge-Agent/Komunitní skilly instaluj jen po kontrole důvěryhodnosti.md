# Komunitní skilly instaluj jen po kontrole důvěryhodnosti

## Trigger
- instalace komunitního skillu
- skill pochází z veřejného katalogu
- neznámý uploader
- skill žádá širší oprávnění

## Core rule
- Pokud skill nepochází z důvěryhodného zdroje → neinstaluj ho bez kontroly

## Decision rules
- Pokud autor není důvěryhodný → nepoužívej skill v ostrém projektu
- Pokud skill žádá široká oprávnění → zkontroluj scope a izolaci
- Pokud existuje varianta od známé organizace → preferuj ji
- Pokud skill čte nebo zapisuje citlivá data → otestuj ho v sandboxu
- Neznámý skill zvyšuje bezpečnostní riziko
- Menší oprávnění snižují dopad chyby

## Use for
- instalace veřejných skillů
- audit pluginů a skillů
- hledání hotového workflow
- práce s citlivými projekty

## Avoid
- anonymní skill v produkčním projektu
- instalace bez přečtení instrukcí
- široká oprávnění kvůli pohodlí
