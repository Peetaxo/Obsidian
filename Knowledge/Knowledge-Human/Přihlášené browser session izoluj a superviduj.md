---
updated: 2026-04-26
created: 2026-04-26
typ: princip
puvod:
  - youtube
  - agenticka-synteza
povaha:
  - pattern-ze-zdroje
  - pracovni-hypoteza
stav: kandidat
duvera: medium
overeno_v_praxi: false
review_poznamka: "Pattern převzatý ze zdrojů; použij jako kandidáta, ne jako dogma, a ověř proti aktuálnímu úkolu."
oblast:
  - browser-automation
  - ai-agent-workflow
pouzij_kdy:
  - automatizace přihlášeného webu
  - persistent browser profile
  - rizikové akce za uživatele
nastroje:
  - Playwright CLI
  - persistent browser profile
  - headed browser
souvisejici:
  - "[[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]"
  - "[[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]]"
  - "[[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]]"
zdroje:
  - "[[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]"
---

# Přihlášené browser session izoluj a superviduj

## Kontext
Použij, když agent automatizuje web, kde je potřeba přihlášení nebo uložené cookies. U přihlášených účtů je důležitá kontrola stavu a lidský dohled při prvním běhu.

## Princip
Přihlášené session lze automatizovat přes persistentní browser profil nebo ruční login handoff. První běh má být supervidovaný a další běhy mají používat uložený stav opatrně.

## Heuristiky

Decision trigger:
- Když web vyžaduje login → použij persistentní profil nebo ruční přihlášení.
- Když automatizace provádí akce za uživatele → spusť první běh v headed režimu.
- Když skript kliká duplicitně nebo moc rychle → přidej kontrolu stavu před akcí.

Pravidla:
- Persistentní cookies snižují tření opakované automatizace.
- Headed první běh zvyšuje kontrolu rizikových akcí.
- Stav UI musí být ověřen před kliknutím.

## Použij při
- komunitních portálech
- interních nástrojích bez API
- školních nebo firemních aplikacích
- automatizaci opakovaných přihlášených úkonů

## Použij s
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|browser automation smyčkou]]
- odděleným browser profilem
- explicitním seznamem povolených akcí
- screenshoty a logy prvního běhu

## Související
- [[AI System/Knowledge/Knowledge-Human/Browser automation jako QA smyčka|Browser automation jako QA smyčka]]
- [[AI System/Knowledge/Knowledge-Human/Automatizační skripty proměňuj ve skills|Automatizační skripty proměňuj ve skills]]
- [[AI System/Knowledge/Knowledge-Human/CLI automatizace šetří tokeny oproti MCP|CLI automatizace šetří tokeny oproti MCP]]

## Zdroje
- [[AI System/Raw/YouTube/Claude Code + Playwright Automates Literally Anything.md]]

## Review
- Stav: Kandidát.
- Důvěra: medium.
- Ověření v praxi: Zatím neověřeno v našem konkrétním projektu.
- Použij jako: pracovní hypotézu ze zdrojů, kterou je potřeba posoudit podle situace.

## Kdy nepoužít
- Když aktuální úkol nemá trigger z heuristik.
- Když by pattern přidal víc režie než snížil riziko, cenu nebo opakovanou práci.

## Anti-pattern
- Spustit headless automatizaci nad přihlášeným účtem bez první vizuální kontroly a ochrany proti duplicitním akcím.

