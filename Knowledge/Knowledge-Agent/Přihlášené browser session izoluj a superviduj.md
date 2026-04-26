# Přihlášené browser session izoluj a superviduj

## Trigger
- automatizace přihlášeného webu
- persistent browser profile
- rizikové akce za uživatele

## Core rule
- Pokud automatizuješ přihlášený účet → použij izolovaný profil a první běh superviduj

## Decision rules
- Pokud web vyžaduje login → použij persistentní profil nebo ruční přihlášení
- Pokud automatizace provádí akce za uživatele → spusť první běh v headed režimu
- Pokud skript kliká duplicitně nebo moc rychle → přidej kontrolu stavu před akcí
- Persistentní cookies snižují tření opakované automatizace
- Headed první běh zvyšuje kontrolu rizikových akcí
- Stav UI musí být ověřen před kliknutím

## Use for
- komunitních portálech
- interních nástrojích bez API
- školních nebo firemních aplikacích
- automatizaci opakovaných přihlášených úkonů

## Avoid
- Spustit headless automatizaci nad přihlášeným účtem bez první vizuální kontroly a ochrany proti duplicitním akcím

