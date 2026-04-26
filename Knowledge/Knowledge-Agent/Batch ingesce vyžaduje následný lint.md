# Batch ingesce vyžaduje následný lint

## Trigger
- hromadné zpracování zdrojů
- import více YouTube transkriptů
- Kontrola konzistence wiki

## Core rule
- Pokud zpracuješ více zdrojů najednou → po ingesci spusť lint wiki

## Decision rules
- Pokud zpracuješ více zdrojů najednou → spusť lint wiki
- Pokud agent vytvoří nové kategorie bez jasného důvodu → zkontroluj strukturu
- Pokud výstupy vypadají nekonzistentně → oprav schema nebo pravidla ingesce
- Batch zvyšuje rychlost ingesce
- Batch snižuje průběžnou supervizi
- Následný lint snižuje dlouhodobý strukturální dluh

## Use for
- zpracování více YouTube videí
- importu starších článků
- migraci poznámek
- automatickém vytváření tematických stránek

## Avoid
- Hromadně ingestovat zdroje a bez kontroly předpokládat, že vzniklá wiki struktura je správná

