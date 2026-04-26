# Pravidelný lint znalostní báze

## Trigger
- wiki rychle roste
- po větší ingesci
- Kontrola odkazů a rozporů
- lokální skript

## Core rule
- Pokud wiki roste nebo prošla batch ingescí → spusť lint konzistence

## Decision rules
- Pokud wiki rychle roste → spusť lint
- Pokud se zdroje časově překrývají nebo odporují → zkontroluj rozpory
- Pokud se pojem opakuje bez vlastní stránky → vytvoř kandidáta na nový blok
- Orphan stránky snižují navigovatelnost
- Zastaralá tvrzení snižují důvěryhodnost wiki
- Chybějící odkazy snižují využitelnost syntézy

## Use for
- pravidelné údržbě wiki
- kontrole po větší ingesci
- přípravě znalostí pro rozhodování
- hledání dalších výzkumných otázek

## Avoid
- Přidávat nové stránky bez kontroly konzistence a propojení

